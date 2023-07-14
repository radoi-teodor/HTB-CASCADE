```bash
nmap -vv --reason -Pn -T4 -sV -p 88 --script="banner,krb5-enum-users" -oN "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp88/tcp_88_kerberos_nmap.txt" -oX "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp88/xml/tcp_88_kerberos_nmap.xml" 10.129.143.95
```

[/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp88/tcp_88_kerberos_nmap.txt](file:///home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp88/tcp_88_kerberos_nmap.txt):

```
# Nmap 7.94 scan initiated Fri Jul 14 15:58:35 2023 as: nmap -vv --reason -Pn -T4 -sV -p 88 --script=banner,krb5-enum-users -oN /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp88/tcp_88_kerberos_nmap.txt -oX /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp88/xml/tcp_88_kerberos_nmap.xml 10.129.143.95
Nmap scan report for 10.129.143.95
Host is up, received user-set (0.059s latency).
Scanned at 2023-07-14 15:58:36 EDT for 16s

PORT   STATE SERVICE      REASON          VERSION
88/tcp open  kerberos-sec syn-ack ttl 127 Microsoft Windows Kerberos (server time: 2023-07-14 19:58:42Z)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Jul 14 15:58:52 2023 -- 1 IP address (1 host up) scanned in 17.19 seconds

```
