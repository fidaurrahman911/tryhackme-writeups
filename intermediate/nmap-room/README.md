TryHackMe — Nmap Room
Date: 2025-11-08
Author: Fida Ur Rahman (account: fidarahman)
Target: 10.10.245.20
Files: 01_Nmap_Completion.png, 02_Nmap_scan_5000ports.png, 03_Nmap_nse_script_output.png

I completed the Nmap room and practiced real reconnaissance on the lab target. First I looked for anonymous FTP using an NSE script:
sudo nmap --script=ftp-anon -p 21 10.10.245.20 -vv
That script did not return any useful anonymous FTP information. The host initially did not respond to simple discovery, so I used -Pn and ran a larger SYN stealth scan to check many ports:
sudo nmap -p1-5000 -sS 10.10.245.20 -Pn -vv
The SYN scan finished and showed the scanned ports as filtered / no response, which means the machine is up but most TCP probes were dropped — likely a firewall or host filtering in place.

What I did and why: I tried the ftp-anon script to see if anonymous FTP access existed. When that gave nothing and the host looked down with normal discovery, I used -Pn to force the scan and confirm the host was reachable. Running a SYN stealth scan helped me test a wide range of ports quickly while being less noisy than full connect scans.

Key findings: the target answered only when forced with -Pn and returned filtered results across the first 5000 TCP ports. No open FTP anonymous access was found. This suggests the target is intentionally hardened or behind packet filters, so normal enumeration shows limited info.

What I learned: use -Pn when hosts block ping; how to run a large -sS scan; how to find and run NSE scripts; and how to interpret “filtered” results (packets dropped, not closed). I saved the room completion badge and terminal screenshots for proof in my portfolio.

Next steps I will take: run targeted -sV -sC scans on common service ports if any appear, try UDP scans for services like DNS if needed, and do web enumeration (Gobuster) if a web port is discovered. I will also save plain text outputs (-oN) next time for clearer records.
