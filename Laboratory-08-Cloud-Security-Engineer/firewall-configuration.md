
# Firewall Configuration

## 1. Allow SSH Connections

The following command allows SSH connections through port 22 so administrators can remotely manage the server.

```bash
sudo ufw allow ssh
```

## 2. Configure the Default Firewall Policies

The following command blocks incoming connections by default:

```bash
sudo ufw default deny incoming
```

The following command allows outgoing connections:

```bash
sudo ufw default allow outgoing
```

## 3. Enable the Firewall

The firewall was activated using:

```bash
sudo ufw enable
```

The configuration was verified using:

```bash
sudo ufw status verbose
```

## 4. Allow TCP Port 8080

The following command creates a rule that allows incoming TCP traffic on port 8080:

```bash
sudo ufw allow 8080/tcp
```

The numbered firewall rules can be checked using:

```bash
sudo ufw status numbered
```

The web service can be tested using:

```bash
curl -i http://localhost:8080
```

## 5. Importance of Allowing SSH Before Enabling UFW

If `sudo ufw enable` is executed before `sudo ufw allow ssh`, remote SSH connections may be blocked by the default-deny incoming policy, potentially locking administrators out of the server.
