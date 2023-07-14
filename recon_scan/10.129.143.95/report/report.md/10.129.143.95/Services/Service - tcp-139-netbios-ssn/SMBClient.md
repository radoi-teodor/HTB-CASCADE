```bash
smbclient -L //10.129.143.95 -N -I 10.129.143.95 2>&1
```

[/home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp139/smbclient.txt](file:///home/kali/Documents/HTB/Cascade/recon_scan/10.129.143.95/scans/tcp139/smbclient.txt):

```
do_connect: Connection to 10.129.143.95 failed (Error NT_STATUS_RESOURCE_NAME_NOT_FOUND)
Anonymous login successful

	Sharename       Type      Comment
	---------       ----      -------
Reconnecting with SMB1 for workgroup listing.
Unable to connect with SMB1 -- no workgroup available


```
