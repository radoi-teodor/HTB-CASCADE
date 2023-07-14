```bash
nmap -vv --reason -Pn -T4 -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp53/tcp_53_dns_nmap.txt" -oX "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp53/xml/tcp_53_dns_nmap.xml" 10.129.143.95
```

[/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp53/tcp_53_dns_nmap.txt](file:///home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp53/tcp_53_dns_nmap.txt):

```
# Nmap 7.94 scan initiated Fri Jul 14 15:58:35 2023 as: nmap -vv --reason -Pn -T4 -sV -p 53 "--script=banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp53/tcp_53_dns_nmap.txt -oX /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp53/xml/tcp_53_dns_nmap.xml 10.129.143.95
Nmap scan report for 10.129.143.95
Host is up, received user-set (0.060s latency).
Scanned at 2023-07-14 15:58:36 EDT for 21s

PORT   STATE SERVICE REASON          VERSION
53/tcp open  domain  syn-ack ttl 127 Microsoft DNS 6.1.7601 (1DB15D39) (Windows Server 2008 R2 SP1)
|_dns-nsec3-enum: Can't determine domain for host 10.129.143.95; use dns-nsec3-enum.domains script arg.
|_dns-nsec-enum: Can't determine domain for host 10.129.143.95; use dns-nsec-enum.domains script arg.
| dns-nsid: 
|_  bind.version: Microsoft DNS 6.1.7601 (1DB15D39)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows_server_2008:r2:sp1

Host script results:
|_dns-brute: Can't guess domain of "10.129.143.95"; use dns-brute.domain script argument.

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Jul 14 15:58:57 2023 -- 1 IP address (1 host up) scanned in 22.27 seconds

```
