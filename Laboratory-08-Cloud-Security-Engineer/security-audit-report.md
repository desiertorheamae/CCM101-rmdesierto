# Security Audit Report

## Checkpoint 2: Security Best Practices

### 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege (PoLP) is a security principle that ensures users, applications, and services are granted only the permissions necessary to perform their designated tasks. Implementing this principle minimizes the risk of unauthorized access and limits the potential impact of compromised accounts or services within a cloud environment.

### 2. Attack Surface

The attack surface refers to the collection of potential entry points through which an unauthorized individual may attempt to access or compromise a server. These entry points include exposed network ports, running services, publicly accessible applications, and user accounts with inadequate security controls. Reducing the attack surface helps minimize potential security vulnerabilities and strengthens the server's overall security posture.

### 3. Default Deny Policy

The Default Deny policy is a security approach in which incoming network traffic is blocked unless explicitly permitted by a defined firewall rule. This approach reduces the likelihood of unauthorized access by ensuring that only approved connections are allowed. Implementing this policy provides an additional layer of protection against unexpected or unauthorized network activity.

## Initial Security Assessment

Before implementing security modifications, the server must undergo an initial assessment to identify active services, exposed network ports, and existing firewall configurations. This assessment establishes a baseline for evaluating the server's security posture before and after the implementation of security controls.

Based on the assessment, firewall rules should be configured to permit only the network traffic required for essential services, including Secure Shell (SSH) for remote administration and port 8080 for the deployed web application. All other incoming connections should remain blocked by default unless explicitly authorized. This approach helps reduce the server's attack surface and supports the implementation of a more secure cloud environment.
