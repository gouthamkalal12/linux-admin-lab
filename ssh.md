# SSH (Secure Shell)

## Connect to Remote Server

```bash
ssh user@server_ip
```

## Connect Using Specific Port

```bash
ssh -p 2222 user@server_ip
```

## Copy File to Remote Server

```bash
scp file.txt user@server_ip:/tmp
```

## Copy File From Remote Server

```bash
scp user@server_ip:/tmp/file.txt .
```

## Generate SSH Key

```bash
ssh-keygen
```

## Copy Public Key

```bash
ssh-copy-id user@server_ip
```

## Restart SSH Service

```bash
systemctl restart sshd
```

## Check SSH Service

```bash
systemctl status sshd
```
