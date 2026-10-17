# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

This laboratory focuses on automating application data backups in a Linux environment. A Bash script was created to compress a sample application directory into a timestamped backup archive, and a cron job was configured to schedule the backup every day at 2:00 AM.

The activity demonstrates how automation can reduce dependence on manual processes and help protect important application data.

## Objectives

- Understand Bash scripts, variables, and cron jobs.
- Create a sample application data directory and test file.
- Write a Bash script to compress application data into a `.tar.gz` archive.
- Use `chmod +x` to make the script executable.
- Execute and verify the backup script.
- Configure a cron job for daily execution at 2:00 AM.
- Document the process and collect screenshots as evidence.

## Commands Executed

### Create the Application Data

```bash
mkdir -p app-data
echo "This is critical client data." > app-data/data.txt
cat app-data/data.txt
```

### Create and Execute the Backup Script

```bash
nano backup.sh
chmod +x backup.sh
./backup.sh
```

### Verify the Backup Archive

```bash
ls -lh backups/
tar -tzf backups/backup_*.tar.gz
```

### Configure and Check Cron

```bash
pwd
crontab -e
crontab -l
service cron status
```

The cron schedule uses the expression `0 2 * * *`, which specifies 2:00 AM every day.

## Skills Learned

- Writing and executing Bash scripts.
- Using variables to manage directory paths and timestamps.
- Creating compressed archives with the `tar` command.
- Managing file permissions with `chmod`.
- Testing backup archives and checking their contents.
- Scheduling recurring tasks with Linux cron.
- Documenting technical procedures in Markdown.
- Using GitHub to maintain and submit laboratory documentation.

## Repository Contents

- `automation-research.md` – Definitions and explanations of automation concepts.
- `backup-script-guide.md` – Backup script, command explanations, testing procedures, and cron configuration.
- `reflection.md` – Personal reflection on the laboratory.
- `screenshots/` – Screenshots documenting the implementation and verification.

## Conclusion

The laboratory demonstrated the basic process of automating application data backups using Bash and cron. The backup script was tested manually, and the daily 2:00 AM schedule was configured. In a production environment, the scheduled execution should also be monitored and verified, and backups should be stored separately from the original application data.
