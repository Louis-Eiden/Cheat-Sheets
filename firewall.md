# Unix Firewall Cheat Sheet

A cheat sheet for Unix firewall commands.

#

<variable> = placeholder for a variable

#

### show iptables

```bash
sudo iptables -L
```

### allow ingoing traffic on specific port

```bash
sudo iptables -A INPUT -p tcp --dport <PORT> -j ACCEPT
```

### allow ingoing traffic on specific port range

```bash
sudo iptables -A INPUT -p tcp --dport <PORT>:<PORT> -j ACCEPT
```

### allow outgoing traffic on specific port

```bash
sudo iptables -A OUTPUT -p tcp --dport <PORT> -j ACCEPT
```

### allow outgoing traffic on specific port range

```bash
sudo iptables -A OUTPUT -p tcp --dport <PORT>:<PORT> -j ACCEPT
```

### allow ingoing traffic from specific IP address on specific port

```bash
sudo iptables -A INPUT -p tcp -s <IP-ADDRESS> --dport <PORT> -j ACCEPT
```

### allow outgoing traffic to specific IP address on specific port

```bash
sudo iptables -A OUTPUT -p tcp -d <IP-ADDRESS> --dport <PORT> -j ACCEPT
```
