# Uncomplicated Firewall (ufw) Cheatsheet

## Installation

```bash
sudo apt install ufw
```

## Basic Usage

### Enable Firewall

```bash
sudo ufw enable
```

### Disable Firewall

```bash
sudo ufw disable
```

### Check Firewall Status and Rules

```bash
sudo ufw status
```

### Allow SSH

```bash
sudo ufw allow ssh
```

### Allow Port

```bash
sudo ufw allow 80
```

### Allow Port Range

```bash
sudo ufw allow 6000:6007/tcp
```

### Allow Specific IP Address

```bash
sudo ufw allow from
```

### Allow Specific IP Address on Specific Port

```bash
sudo ufw allow from to any port
```

### show all rules

```bash
sudo ufw show raw
```

### Delete Rule

```bash
sudo ufw delete allow ssh
```
