```bash
nmap -vv --reason -Pn -T4 -sV -p 49170 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp49170/tcp_49170_rpc_nmap.txt" -oX "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp49170/xml/tcp_49170_rpc_nmap.xml" 10.129.143.95
```

[/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp49170/tcp_49170_rpc_nmap.txt](file:///home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp49170/tcp_49170_rpc_nmap.txt):

```
# Nmap 7.94 scan initiated Fri Jul 14 16:00:08 2023 as: nmap -vv --reason -Pn -T4 -sV -p 49170 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp49170/tcp_49170_rpc_nmap.txt -oX /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp49170/xml/tcp_49170_rpc_nmap.xml 10.129.143.95
Nmap scan report for 10.129.143.95
Host is up, received user-set (0.059s latency).
Scanned at 2023-07-14 16:00:08 EDT for 70s

PORT      STATE SERVICE REASON          VERSION
49170/tcp open  msrpc   syn-ack ttl 127 Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Jul 14 16:01:18 2023 -- 1 IP address (1 host up) scanned in 69.95 seconds

```
