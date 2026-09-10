## Checkpoint 7 – Linux Investigation

I used the KillerCoda Linux environment to check the operating system, CPU information, memory, and disk space. The commands used were `cat /etc/os-release`, `lscpu`, `free -h`, and `df -h`.

### Linux Server Information

- **Operating System:** Ubuntu 24.04.4 LTS
- **CPU:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
- **CPU Cores:** 1
- **Memory:** 1.9 GiB
- **Disk Space:** 19 GB total

### Cloud Services That Could Host the Linux Server

If this Linux server were migrated to the cloud, it could be hosted using a virtual machine service from any of the three major cloud providers.

| Cloud Provider | Service |
|---|---|
| AWS | Amazon EC2 |
| Microsoft Azure | Azure Virtual Machines |
| GCP | Compute Engine |

These services can provide virtual machines that run Linux operating systems. The choice would depend on the organization's budget, performance requirements, existing systems, and preferred cloud provider.

### Evidence

![KillerCoda Linux Terminal](screenshots/killercoda-terminal.png)
