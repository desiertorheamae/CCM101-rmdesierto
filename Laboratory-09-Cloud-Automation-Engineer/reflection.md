# Laboratory Reflection

This laboratory helped me understand the importance of automation in cloud computing and Linux system administration. I created a sample application data directory and developed a Bash script to compress its contents into a timestamped backup archive.

I learned how variables make scripts easier to maintain and how the `tar` command can be used to create compressed backup files. Testing the script and checking the archive contents helped me confirm that the expected application files were included in the backup.

I also learned how to configure a cron job to schedule a task automatically. By using the cron expression `0 2 * * *`, I configured the backup script to run every day at 2:00 AM without requiring someone to start it manually.

This activity showed me how automation can reduce human error and help protect important application data. I also learned that a scheduled backup must be monitored and verified to ensure that it actually runs successfully. In a real cloud environment, I would improve the process by checking for backup errors, keeping older backup copies, and storing backups in a separate location.

Overall, this laboratory improved my practical knowledge of Bash scripting, file compression, cron scheduling, and automated data protection.
