# <a href='https://www.vulnhub.com/entry/dc-9,412/' target="blank">DC: 9</a>

## <a href='/walk-through/machines-for-oscp/vulnhub/DC-9/nmapAutomator/' target="blank">Enumeration</a>

### Quick Scanning

``` bash
┌──(Hades㉿192.168.110.131)-[0.6:13.4]~
└─$ nmap -p- --min-rate 3000 192.168.110.138
Starting Nmap 7.91 ( https://nmap.org ) at 2021-01-28 02:10 EST
Nmap scan report for 192.168.110.138
Host is up (0.0013s latency).
Not shown: 65534 closed ports
PORT   STATE SERVICE
80/tcp open  http

Nmap done: 1 IP address (1 host up) scanned in 2.54 seconds
```