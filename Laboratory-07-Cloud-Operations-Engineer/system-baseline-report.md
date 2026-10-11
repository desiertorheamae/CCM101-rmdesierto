# System Baseline Report

## 1. Memory (RAM) Check

Command used:

`free -h`

- **Total RAM:** [Enter the total RAM shown in your terminal]
- **Used RAM:** [Enter the used RAM]
- **Available RAM:** [Enter the available RAM]

Screenshot: `screenshots/memory-check.png`

## 2. Disk Storage Check

Command used:

`df -h /`

- **Root filesystem (/):** [Enter the filesystem size]
- **Used storage:** [Enter the used storage]
- **Available storage:** [Enter the available storage]
- **Usage percentage:** [Enter the percentage]

Screenshot: `screenshots/disk-check.png`

## 3. CPU and Process Monitoring

Command used:

`top`

The `top` command was used to observe CPU load, memory utilization, and active processes over several seconds.

## 4. Importance of Disk Monitoring

Checking disk space before a massive traffic surge is critical because insufficient storage can prevent applications from writing logs, caching data, or saving files, potentially causing service interruptions.
