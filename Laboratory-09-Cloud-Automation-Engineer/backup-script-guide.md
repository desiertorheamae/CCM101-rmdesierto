# Backup Script Guide

## 1. Introduction

This guide explains how to create, execute, and test a Bash script that automatically backs up application data. The script compresses the application data directory into a timestamped archive to help protect important files from accidental loss.

## 2. Creating the Application Data

The following commands create a sample application directory and a text file containing test data.

```bash
mkdir -p app-data
echo "This is critical client data." > app-data/data.txt
```

The `cat` command can be used to verify the contents of the file.

```bash
cat app-data/data.txt
```

Expected output:

```text
This is critical client data.
```

## 3. Creating the Backup Script

Create the script using the Nano text editor.

```bash
nano backup.sh
```

Enter the following Bash code:

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

Save the file using `Ctrl + O`, press `Enter`, and exit using `Ctrl + X`.

## 4. Executing the Script

Make the script executable and run it.

```bash
chmod +x backup.sh
./backup.sh
```

The script displays a message when the backup process starts and another message when the command sequence finishes.

## 5. Verifying the Backup

List the generated backup archives.

```bash
ls -lh backups/
```

Display the contents of the compressed archive.

```bash
tar -tzf backups/backup_*.tar.gz
```

To verify the archived text file, run the following command using the actual archive filename:

```bash
tar -xOzf backups/backup_20261017_152502.tar.gz app-data/data.txt
```

The expected output is:

```text
This is critical client data.
```

The terminal test showed that a compressed backup archive was created and contained `app-data/` and `app-data/data.txt`. The archived text can also be checked to confirm that the expected data was preserved.

## 6. Scheduling the Backup with Cron

The script is configured to run automatically every day at 2:00 AM using the root user's crontab.

```cron
0 2 * * * /bin/bash /root/backup.sh >> /root/backup-cron.log 2>&1
```

The five scheduling fields specify the minute, hour, day of the month, month, and day of the week. The expression `0 2 * * *` means that the command is scheduled for 2:00 AM every day.

The command redirects standard output and error messages to `/root/backup-cron.log`.

## 7. Checking the Cron Configuration

Display the current cron schedule.

```bash
crontab -l
```

Check the cron service status.

```bash
service cron status
```

The cron configuration was entered in the KillerCoda Ubuntu environment. The service status and actual scheduled execution should be checked separately.

## 8. Test Results

- Application data file: Created successfully.
- Backup script execution: Successful in the manual test.
- Backup archive: Created successfully.
- Archive contents: Confirmed to include the application directory and text file.
- Cron schedule: Configured for daily execution at 2:00 AM.
- Automatic scheduled execution: Requires verification after the scheduled time.

## 9. Conclusion

The laboratory demonstrated how Bash scripting and cron scheduling can automate routine backup operations. Compressing application data into timestamped archives helps reduce manual work and supports data protection. In a production environment, backup scripts should also check for errors, retain multiple backup versions, and store copies in a separate location to improve reliability.
