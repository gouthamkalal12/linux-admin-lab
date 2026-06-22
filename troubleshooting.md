# Linux Troubleshooting

## Server is Slow

### Check CPU Usage

```bash
top
```

### Check Memory Usage

```bash
free -h
```

### Check Disk Usage

```bash
df -h
```

### Check Running Processes

```bash
ps -ef
```

## SSH Not Working

### Check SSH Service

```bash
systemctl status sshd
```

### Check Port 22

```bash
ss -tulnp | grep 22
```

## Disk Full

### Find Large Directories

```bash
du -sh /*
```

### Find Large Files

```bash
find / -type f -size +500M
```

## Network Issues

### Check Connectivity

```bash
ping google.com
```

### Check DNS Resolution

```bash
nslookup google.com
```
