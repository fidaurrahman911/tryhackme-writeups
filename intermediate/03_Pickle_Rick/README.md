# 🥒 Pickle Rick

## 📊 Challenge Information

**Platform:** TryHackMe  
**Difficulty:** Intermediate  
**Category:** Web Exploitation | Linux  
**Estimated Completion Time:** ~45 Minutes

---

# 📌 Objective

The objective of this room was to practice web application enumeration, Linux command-line navigation, and basic privilege escalation techniques by helping Rick locate the three secret ingredients needed to transform himself back into a human.

Through this challenge, I explored a vulnerable web application, analyzed hidden resources, and used Linux commands to retrieve sensitive files while following a structured penetration testing methodology.

---

# 🛠 Skills Practiced

- Web Application Enumeration
- Nmap Scanning
- Source Code Inspection
- robots.txt Enumeration
- Linux Command Line
- File System Navigation
- Command Execution
- Information Gathering
- Problem Solving

---

# 💻 Tools Used

- Nmap
- Firefox Browser
- Kali Linux
- Bash Terminal

---

# 🔍 Methodology

### 1. Enumeration

I started by identifying open ports and services running on the target machine.

```bash
sudo nmap -A -T5 -Pn TARGET_IP
```

The scan revealed an HTTP service, which became the primary target for further investigation.

### 2. Web Enumeration

After accessing the website, I inspected the HTML source code and discovered a hidden username.

I then explored the **robots.txt** file, which revealed another important clue that helped me progress further into the challenge.

### 3. Exploitation

After successfully accessing the command panel, I navigated the Linux file system using commands such as:

```bash
ls
cd
pwd
cat
find
sudo
```

By carefully exploring directories and reading files, I successfully located all three secret ingredients required to complete the room.

---

# 📚 What I Learned

This room reinforced several important cybersecurity concepts:

- Reconnaissance should always be the first step before exploitation.
- Small files like **robots.txt** or HTML comments may expose sensitive information.
- Linux command-line skills are essential for penetration testing.
- Careful enumeration often leads to successful exploitation more effectively than rushing into attacks.

---

# 📷 Screenshots

| Screenshot | Description |
|------------|-------------|
| 01_Nmap_Scan.png | Initial Nmap scan against the target machine |
| 02_Second_Flag.png | Discovery of the second secret ingredient |
| 03_Third_Flag.png | Retrieval of the final secret ingredient |
| 04_Room_Completed.png | Successful completion of the room |

---

# 🎯 Outcome

✅ Successfully completed the **Pickle Rick** room.

This challenge strengthened my practical skills in web enumeration, Linux navigation, reconnaissance, and information gathering while improving my overall penetration testing methodology.

---

# 🚀 Next Learning Goal

To continue building my practical cybersecurity skills, my next focus areas are:

- Linux Privilege Escalation
- Web Application Security
- Authentication & Authorization Testing
- Active Directory Fundamentals

Following a structured learning path allows me to build knowledge progressively rather than solving random CTF challenges.

---

# 👨‍💻 Author

## Fida Ur Rahman

Aspiring Computer Science student from Pakistan with a strong interest in cybersecurity, artificial intelligence, and software development. I enjoy solving real-world security challenges, building practical projects, and documenting my hands-on learning journey through Capture The Flag (CTF) exercises and cybersecurity labs.

### 🌐 Connect with Me

- **GitHub:** https://github.com/fidaurrahman911
- **LinkedIn:** *(Given in my github profile)
- **Portfolio:** *(Given in my Github Profile)

---

## 📌 About This Repository

This repository documents my cybersecurity learning journey through TryHackMe. Every write-up highlights the methodology, tools, key concepts, and lessons learned from each room. My goal is to continuously improve my practical skills while building a professional portfolio that showcases my growth as a future Computer Science student and cybersecurity professional.
