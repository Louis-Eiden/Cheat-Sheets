# Security Cheatsheet

---
## **UNDER CONSTRUCTION**
---

A cheatsheet for security related stuff.

#

## Table of Contents

- [Fix Docker security issues on VPS](#fix-docker-security-issues-on-vps)
  - [Set up firewall](#set-up-firewall)
  - [Configure Docker to use iptables](#configure-docker-to-use-iptables)

#

## Fix Docker security issues on VPS

[source](https://www.techrepublic.com/article/how-to-fix-the-docker-and-ufw-security-flaw/)

### 1. Set up firewall

```bash
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw enable
```

### 2. Configure Docker to use iptables

```bash
sudo nano /etc/default/docker
```

### 3. Add the following line:

```bash
DOCKER_OPTS="--iptables=false"
```

Restart Docker:

```bash
sudo systemctl restart docker
```

#
