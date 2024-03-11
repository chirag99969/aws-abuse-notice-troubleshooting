### Troubleshooting for AWS Abuse notice for Ec2 Instances

```
telnet 1.1.1.108 80
```

```
curl http://169.254.169.254/latest/meta-data/public-ipv4 1.1.1.108
```

```
netstat -tulpn | grep :80
```

```
lsof -i :80 | grep LISTEN
```

```
curl http://1.1.1.108
```

```
nmap -v --open -p- 1.1.91.108
```

```
nmap -sV -version-all --script http-open-proxy -p80 1.1.1.108
```

```
netstat -antp | grep :22 -c
```

```
ps ax | grep 5084
```

```
kill -9 5084
```

```
ps alx | grep 17791
```

```
kill -9 17791
```

```
netstat -antp | grep :22
```
