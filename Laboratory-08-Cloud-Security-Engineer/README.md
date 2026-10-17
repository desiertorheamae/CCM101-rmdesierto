# Laboratory 08: Cloud Security Engineer

## 1. Mission Overview

This laboratory focuses on securing an Ubuntu server using Docker, Nginx, and the Uncomplicated Firewall (UFW). It demonstrates how firewall rules and proper port management help protect a server from unauthorized network access.

## 2. Objectives

- Understand Least Privilege, attack surface reduction, and Default Deny.
- Deploy and test an Nginx web application using Docker.
- Configure UFW to deny incoming traffic by default.
- Allow SSH on port 22 and TCP traffic on port 8080.
- Verify firewall rules and application connectivity.
- Document the procedures and results using Markdown.

## 3. Commands Executed

```bash
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl -i http://localhost:8080
```

## 4. Laboratory Files

- `security-audit-report.md` – Documents security principles and audit findings.
- `firewall-configuration.md` – Records firewall commands and configuration.
- `reflection.md` – Presents the lessons learned from the mission.
- `screenshots/` – Contains evidence of application deployment and firewall verification.

## 5. Skills Learned

- Configuring Linux firewalls using UFW.
- Managing network ports and access rules.
- Deploying web applications using Docker and Nginx.
- Testing application connectivity using `curl`.
- Writing technical documentation using Markdown.

## 6. Conclusion

This laboratory improved my understanding of server security, firewall configuration, and network access control. It demonstrated the importance of restricting unnecessary connections and allowing only authorized traffic to reduce security risks in cloud environments.
