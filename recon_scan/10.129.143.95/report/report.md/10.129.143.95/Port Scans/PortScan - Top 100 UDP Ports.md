```bash
nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/_top_100_udp_nmap.txt" -oX "/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/xml/_top_100_udp_nmap.xml" 10.129.143.95
```

[/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/_top_100_udp_nmap.txt](file:///home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.94 scan initiated Fri Jul 14 15:56:42 2023 as: nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/_top_100_udp_nmap.txt -oX /home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/xml/_top_100_udp_nmap.xml 10.129.143.95
Nmap scan report for 10.129.143.95
Host is up, received user-set (0.062s latency).
Scanned at 2023-07-14 15:56:42 EDT for 1782s
Not shown: 98 open|filtered udp ports (no-response)
PORT    STATE SERVICE REASON               VERSION
53/udp  open  domain  udp-response ttl 127 Microsoft DNS 6.1.7601 (1DB15D39) (Windows Server 2008 R2 SP1)
| dns-nsid: 
|_  bind.version: Microsoft DNS 6.1.7601 (1DB15D39)
123/udp open  ntp     udp-response ttl 127 NTP v3
| ntp-info: 
|_  receive time stamp: 2023-07-14T20:03:35
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: specialized|VoIP phone|general purpose|phone
Running: Allen-Bradley embedded, Atcom embedded, Microsoft Windows 7|8|Phone|XP|2012, Palmmicro embedded, VMware Player
OS CPE: cpe:/h:allen-bradley:micrologix_1100 cpe:/h:atcom:at-320 cpe:/o:microsoft:windows_7 cpe:/o:microsoft:windows_8 cpe:/o:microsoft:windows cpe:/o:microsoft:windows_xp::sp3 cpe:/o:microsoft:windows_server_2012 cpe:/a:vmware:player
OS details: Allen Bradley MicroLogix 1100 PLC, Atcom AT-320 VoIP phone, Microsoft Windows Embedded Standard 7, Microsoft Windows 8.1 Update 1, Microsoft Windows Phone 7.5 or 8.0, Microsoft Windows XP SP3 or Windows 7 or Windows Server 2012, Palmmicro AR1688 VoIP module, VMware Player virtual NAT device
TCP/IP fingerprint:
OS:SCAN(V=7.94%E=4%D=7/14%OT=%CT=%CU=%PV=Y%DS=2%DC=T%G=N%TM=64B1AF70%P=x86_
OS:64-pc-linux-gnu)SEQ(II=I)U1(R=N)IE(R=Y%DFI=N%TG=80%CD=Z)

Network Distance: 2 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows_server_2008:r2:sp1

Host script results:
|_clock-skew: 8s

TRACEROUTE (using port 53/udp)
HOP RTT      ADDRESS
1   59.36 ms 10.10.14.1
2   63.20 ms 10.129.143.95

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Jul 14 16:26:24 2023 -- 1 IP address (1 host up) scanned in 1781.81 seconds

```
