
# Metasploit: Introduction (TryHackMe)

## Difficulty
🟡 Intermediate

## Room Link
https://tryhackme.com/room/metasploitintro

---

# Objective

Learn the fundamentals of the Metasploit Framework, one of the world's most widely used penetration testing frameworks.

This room introduces:

- What Metasploit is
- Framework architecture
- Modules
- Payloads
- Exploits
- Auxiliary modules
- Encoders
- Basic usage

---

# What I Learned

## 1. What is Metasploit?

Metasploit Framework is an open-source penetration testing framework used to:

- Discover vulnerabilities
- Develop exploits
- Deliver payloads
- Perform post-exploitation

It simplifies penetration testing by providing thousands of ready-made modules.

---

## 2. Modules

Metasploit organizes functionality into modules.

Main categories include:

- Exploit
- Payload
- Auxiliary
- Encoder
- NOP
- Post

Each serves a different purpose during an assessment.

---

## 3. Exploits

Exploit modules take advantage of known software vulnerabilities.

Example workflow:

1. Select exploit
2. Configure target
3. Select payload
4. Launch exploit

---

## 4. Payloads

Payloads execute after successful exploitation.

Common payloads include:

- Reverse Shell
- Bind Shell
- Meterpreter

Meterpreter provides an interactive shell with advanced post-exploitation capabilities.

---

## 5. Auxiliary Modules

Auxiliary modules perform tasks without exploiting vulnerabilities.

Examples:

- Port scanning
- Banner grabbing
- SMB enumeration
- FTP login testing
- SNMP enumeration

---

## 6. Encoders

Encoders modify payloads to help evade basic signature detection.

They are useful in certain situations but are not guaranteed to bypass modern antivirus solutions.

---

## 7. Basic Metasploit Workflow

Typical penetration testing workflow:

1. Start Metasploit
2. Search for exploit
3. Select module
4. Configure target
5. Configure payload
6. Verify settings
7. Execute exploit
8. Perform post-exploitation

---

# Skills Gained

- Understanding the Metasploit Framework
- Identifying different module types
- Selecting exploits and payloads
- Learning penetration testing workflow
- Familiarity with exploitation concepts
- Basic post-exploitation understanding

---

# Key Takeaways

This room provided a strong introduction to the Metasploit Framework and demonstrated how security professionals organize exploits, payloads, and post-exploitation activities during penetration testing.

Understanding Metasploit is essential for ethical hackers and penetration testers.

---

# Suggestions

After completing this room, I plan to:

- Complete Metasploit: Exploitation
- Learn Meterpreter in depth
- Practice exploiting intentionally vulnerable machines
- Combine Metasploit with Nmap results
- Study privilege escalation after exploitation
- Continue documenting every room on GitHub for future reference

---

## Screenshots

### Room Completed

![Room Completed](screenshots/01_Room_Completed.png)

---

### Completion Badge

![Completion Badge](screenshots/02_Completion_Badge.png)

---
