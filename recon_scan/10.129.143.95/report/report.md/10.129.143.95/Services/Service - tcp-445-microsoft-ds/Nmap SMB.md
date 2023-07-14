```bash
nmap -vv --reason -Pn -T4 -sV -p 445 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp445/tcp_445_smb_nmap.txt" -oX "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp445/xml/tcp_445_smb_nmap.xml" 10.129.143.95
```

[/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp445/tcp_445_smb_nmap.txt](file:///home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp445/tcp_445_smb_nmap.txt):

```
# Nmap 7.94 scan initiated Fri Jul 14 15:58:35 2023 as: nmap -vv --reason -Pn -T4 -sV -p 445 "--script=banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp445/tcp_445_smb_nmap.txt -oX /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp445/xml/tcp_445_smb_nmap.xml 10.129.143.95
Nmap scan report for 10.129.143.95
Host is up, received user-set (0.062s latency).
Scanned at 2023-07-14 15:58:36 EDT for 45s

PORT    STATE SERVICE       REASON          VERSION
445/tcp open  microsoft-ds? syn-ack ttl 127
|_smb-enum-services: ERROR: Script execution failed (use -d to debug)

Host script results:
| smb2-capabilities: 
|   2:0:2: 
|     Distributed File System
|   2:1:0: 
|     Distributed File System
|     Leasing
|_    Multi-credit operations
| smb2-security-mode: 
|   2:1:0: 
|_    Message signing enabled and required
|_smb-print-text: false
| smb-mbenum: 
|_  ERROR: Failed to connect to browser service: Could not negotiate a connection:SMB: Failed to receive bytes: ERROR
| smb-protocols: 
|   dialects: 
|     2:0:2
|_    2:1:0
| smb2-time: 
|   date: 2023-07-14T19:58:57
|_  start_date: 2023-07-14T19:53:43
|_smb-vuln-ms10-061: Could not negotiate a connection:SMB: Failed to receive bytes: ERROR

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Jul 14 15:59:21 2023 -- 1 IP address (1 host up) scanned in 45.64 seconds

```
