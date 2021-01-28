# All Port Scan

## Normal Scanning

### TCP

``` bash
nmap -p- -T3 $ip -o all_tcp.nmap
```

### UDP

``` bash
sudo nmap -sU -p- $ip -o all_udp.nmap
```

### Services Enum

``` bash
ports=$(cat all_tcp.nmap | grep ^[0-9] | cut -d '/' -f1 | tr '\n' ',' | sed s/,$//); echo $ports
```

``` bash
nmap -sC -sV -p$ports $ip
```

## Quick Scanning

### TCP

``` bash
nmap -p- --min-rate 3000 192.168.110.136
```