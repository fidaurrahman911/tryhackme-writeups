 Linux Fundamentals Part 1 — TryHackMe
Date: 23-10-2025
Author:Fida Ur Rahman  
TryHackMe username: fidarahman

## Objective
Complete the TryHackMe "Linux Fundamentals Part 1" room to learn and practice basic Linux commands and system concepts needed for cybersecurity labs.

## Summary of what I did
I completed the full Linux Fundamentals Part 1 learning path on TryHackMe. The module covered important topics such as files and directories, file permissions, process management, basic networking commands, and simple file editing in the terminal. I followed the walkthrough, completed the exercises, and studied the examples to build practical understanding.

Commands and concepts reviewed
(These are the key commands and concepts I reviewed and practiced in my local Kali environment.)
- `ls -la` — list files and show permissions and hidden files.  
- `pwd` — print working directory.  
- `cat filename` / `less filename` — view file contents.  
- `chmod` / `chown` — modify file permissions and ownership.  
- `sudo -l` — check allowed sudo commands for current user.  
- `ps aux` / `top` — view running processes.  
- `ss -tulpn` — list listening services and open ports.  
- `nano` / `vim` — basic text file editing.

 Key observations / learning points
- File permissions (rwx and octal notation) are central to access control and privilege escalation.  
- Enumeration (checking running processes and network sockets) is the first step when approaching a target.  
- Small command-line skills (reading files, checking services) are required for almost every lab and are essential to speed up troubleshooting and analysis.

 Outcome
- I completed the TryHackMe room (completion screenshot saved as `01_Linux_Fundamentals_Completion.png`).  
- I am now comfortable running basic Linux commands and interpreting their outputs.  
- I can perform initial enumeration steps on lab machines and prepare for privilege escalation practice.

 Next steps
1. Practice `sudo -l` and SUID discovery (`find / -perm -4000 -type f 2>/dev/null`) on a local VM.  
2. Do 2 small HTB/THM enumeration machines and create full writeups with command outputs and screenshots.  
3. Start a focused Privilege Escalation study after completing practice machines.

 Attachments (in this folder)
- `Completion.png`  (TryHackMe completion screenshot)  

