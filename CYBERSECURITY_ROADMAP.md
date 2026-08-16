# The Ultimate Free Cyber Security Roadmap (2026 Edition)

> A structured, explanation-first roadmap for learning cybersecurity from zero — using only free resources.
> Companion repo: **The Ultimate Free AI Roadmap** 

---

## 00. Introduction

### Why does this roadmap exist?
Most roadmaps are just a wall of links. You get a list of 40 websites and no idea *why* any of them matter or *in what order* to use them. This repo tries to do something different: every section explains **why the topic matters**, **what exactly to learn**, gives you **free resources**, **practice platforms**, **book recommendations**, a **mini project**, and a checklist to tell you **when you're ready to move on**.

### The core idea
Cybersecurity is not a standalone skill. It's **applied Computer Science**. A buffer overflow only makes sense if you understand memory. Malware analysis only makes sense if you understand operating systems. Network attacks only make sense if you understand protocols. So this roadmap builds real Computer Science knowledge *inside* the security path, instead of skipping straight to "hacking."

### How to use this repo
Go through the sections roughly in order (01 → 20). Each section is self-contained — read the "Why," study the "What," work through the free resources, do the practice labs, build the mini project, then check the "ready to move on" list before continuing.

### Suggested weekly rhythm

| Day | Focus |
|---|---|
| Mon | Computer Science / theory |
| Tue | Reading + note-taking on the week's topic |
| Wed | Hands-on labs |
| Thu | Practice platform (TryHackMe / HTB / PicoCTF) |
| Fri | Continue labs / start the mini project |
| Sat | Finish the mini project |
| Sun | Write the project README, push to GitHub, review the week |

---

## 01. Programming

### Why should I learn this?
Every tool you'll ever use in security was written by someone who could program, and eventually you'll need to write your own — a custom scanner, a small exploit script, an automation tool. Programming is the one skill that shows up in literally every other section of this roadmap.

### What should I learn?
- Variables, loops, functions, data types
- File I/O and basic string manipulation
- Working with libraries and virtual environments
- Basic scripting for automation

### Free Resources
- [CS50P — Introduction to Programming with Python (Harvard)](https://cs50.harvard.edu/python/)
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/) — free full book
- [Exercism](https://exercism.org/) — free mentored coding exercises

### Practice Platforms
- [HackerRank](https://www.hackerrank.com/)
- [LeetCode](https://leetcode.com/) (Easy problems for now)

### Recommended Books
- *Automate the Boring Stuff with Python* (Al Sweigart) — free online
- *Python Crash Course* (Eric Matthes) — commercial, check library access

### Mini Projects
- File organizer script
- Simple password generator
- Basic CSV log parser

### ✅ When am I ready to move on?
- [ ] I can write a script without constantly looking up basic syntax
- [ ] I understand functions, loops, and conditionals without hesitation
- [ ] I've solved at least 20–30 small problems on HackerRank/Exercism

---

## 02. Linux

### Why should I learn this?
Linux is the operating system behind most servers, cloud platforms, cybersecurity labs, and penetration testing distributions (like Kali). Learning Linux isn't about memorizing commands — it's about understanding how an operating system actually works underneath the GUI.

### What should I learn?
- File system structure
- Permissions (`chmod`, `chown`, ownership model)
- Processes and process management
- Basic networking commands
- Bash and shell scripting
- Pipes, `grep`, `awk`, `sed`

### Free Resources
- [Linux Journey](https://linuxjourney.com/) — free, structured, beginner-friendly
- [linuxdersleri.net](https://www.linuxdersleri.net/) — free, well-structured Linux course
- [ExplainShell](https://explainshell.com/) — paste any command and see what every part does

### Practice Platforms
- [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) — free wargame, learn the terminal level by level
- [CMD Challenge](https://cmdchallenge.com/) — free bite-sized bash challenges

### Recommended Books
- *The Linux Command Line* (William Shotts) — free PDF from the author at linuxcommand.org
- *How Linux Works* (Brian Ward) — commercial, check library access

### Mini Projects
- File organizer that sorts files by type
- Log parser script
- Simple backup script
- Basic system resource monitor

### ✅ When am I ready to move on?
- [ ] I completed all Bandit levels (or at least 20+)
- [ ] I can navigate, search, and manipulate files entirely from the terminal
- [ ] I understand file permissions and can explain `chmod 755` without looking it up

---

## 03. Networking

### Why should I learn this?
Before you can attack or defend anything, you need to understand how computers actually talk to each other. A huge percentage of real vulnerabilities exist because a protocol was misunderstood or misconfigured — not because of some exotic zero-day.

### What should I learn?
- OSI model & TCP/IP model
- DNS, HTTP, HTTPS, TLS
- TCP vs UDP
- Routing & switching basics
- ARP and how MITM attacks exploit it

### Free Resources
- [Professor Messer — Network+ course](https://www.professormesser.com/) — free full video series
- [Cisco Skills For All](https://www.netacad.com/skills-for-all) — free Cisco networking courses
- [Practical Networking](https://www.practicalnetworking.net/) — free articles that build strong intuition
- [Wireshark](https://www.wireshark.org/) — free, install it and inspect your own traffic
- [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) — free network simulator

### Practice Platforms
- Packet Tracer labs (build your own small networks)
- Wireshark labs (capture and analyze real traffic)
- [TryHackMe](https://tryhackme.com/) — free networking-focused rooms

### Recommended Books
- *Computer Networking: A Top-Down Approach* (Kurose & Ross) — commercial, check library/university access
- *TCP/IP Illustrated* (W. Richard Stevens) — commercial, check library access

### Mini Projects
- Ping scanner
- Port scanner
- Packet sniffer (using raw sockets or Scapy)
- ARP scanner
- Simple DNS resolver

### ✅ When am I ready to move on?
- [ ] I can explain the TCP 3-way handshake from memory
- [ ] I can read a Wireshark capture and identify HTTP requests/responses
- [ ] I understand what ARP spoofing is and why it works

---

## 04. Computer Science

### Why should I learn this?
This is the section most roadmaps get wrong — they either skip it entirely or make it a separate track you're supposed to do "someday." Don't skip it. Everything downstream depends on it:

```
Buffer Overflow → Memory → Stack → Heap → Assembly → Operating System
```

If you don't understand memory and how an OS manages processes, buffer overflows, privilege escalation, and malware analysis will always feel like memorized magic instead of things you actually understand.

### What should I learn?
- Computer architecture: CPU, RAM, cache, registers, stack, heap
- Operating systems: processes, threads, system calls, virtual memory, file systems, scheduling
- Data structures: arrays, linked lists, stacks, queues, hash tables, trees, graphs
- Algorithms: sorting, searching, DFS/BFS, basic dynamic programming
- Databases: SQL, joins, indexing, normalization

### Free Resources
- [OSTEP — Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/) — completely free, excellent
- [Neso Academy — Computer Organization (YouTube)](https://www.youtube.com/c/nesoacademy) — free
- [NeetCode](https://neetcode.io/) — free tier, data structures & algorithms
- [PostgreSQL Official Tutorial](https://www.postgresql.org/docs/current/tutorial.html) — free

### Practice Platforms
- [LeetCode](https://leetcode.com/) — Easy → Medium problems

### Recommended Books
- *Computer Systems: A Programmer's Perspective* (Bryant & O'Hallaron) — commercial, check library access
- *OSTEP* — free, linked above

### Mini Projects
- Small C programs that demonstrate stack/heap memory usage (inspect with `gdb`)
- Mini shell implementation
- Simple thread pool
- Blog API backed by a real database

### ✅ When am I ready to move on?
- [ ] I can explain the difference between stack and heap memory
- [ ] I understand what a system call is and can name a few
- [ ] I've solved 50+ Easy problems on LeetCode
- [ ] I can write basic SQL joins without help

---

## 05. Web

### Why should I learn this?
You cannot break what you don't understand. The vast majority of real-world attack surface today is web applications — so before "web security," you need to understand how the web actually works.

### What should I learn?
- How browsers and servers communicate (requests/responses, headers, cookies)
- HTML/CSS/JS basics
- How client-side and server-side rendering differ
- Sessions, cookies, and how state is maintained over HTTP

### Free Resources
- [MDN Web Docs](https://developer.mozilla.org/en-US/) — free, the standard reference for web technologies
- [freeCodeCamp — Responsive Web Design](https://www.freecodecamp.org/learn/2022/responsive-web-design/) — free

### Practice Platforms
- Build and deploy a static site for free (GitHub Pages)

### Recommended Books
- *Eloquent JavaScript* (Marijn Haverbeke) — free online at eloquentjavascript.net

### Mini Projects
- A static personal portfolio page
- A simple contact form (no backend yet — just front-end validation)

### ✅ When am I ready to move on?
- [ ] I understand the request/response cycle
- [ ] I can read HTTP headers and know what cookies do
- [ ] I've built at least one static site

---

## 06. Backend Basics

### Why should I learn this?
A huge amount of real security work — web app pentesting, API security, DevSecOps — requires understanding how the thing you're attacking was actually built. You won't recognize a broken authentication flow if you've never built one yourself.

### What should I learn?
- REST APIs
- Authentication & authorization (sessions, JWT)
- CRUD operations
- Input validation
- Connecting a backend to a database

### Free Resources
- [FastAPI Official Documentation](https://fastapi.tiangolo.com/) — free, excellent docs
- [Docker — Get Started guide](https://docs.docker.com/get-started/) — free

### Practice Platforms
- Build and test your own API locally with Postman/Insomnia (both have free tiers)

### Recommended Books
- No single definitive free book here — official framework docs (linked above) are the best free resource

### Mini Projects
- Login/authentication system with JWT
- File upload service
- Dockerized REST API

### ✅ When am I ready to move on?
- [ ] I've built a working API with at least one authenticated route
- [ ] I understand what JWT is and how it's validated
- [ ] I can containerize an app with Docker

---

## 07. Web Security

### Why should I learn this?
Now it all connects. You understand networking, the web, and backend development — so web vulnerabilities will actually make sense instead of feeling like following a script.

### What should I learn?
- OWASP Top 10 (SQL Injection, XSS, CSRF, SSRF, Broken Access Control, etc.)
- Authentication & session vulnerabilities
- File upload vulnerabilities
- API security basics

### Free Resources
- [OWASP Top 10](https://owasp.org/www-project-top-ten/) — free, the standard reference
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — completely free, includes the free Burp Suite Community Edition; arguably the single best free web security resource that exists
- [OWASP WebGoat](https://owasp.org/www-project-webgoat/) — free, intentionally vulnerable app to practice on
- [DVWA (Damn Vulnerable Web Application)](https://github.com/digininja/DVWA) — free, self-hosted vulnerable app
- [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) — free, modern intentionally-vulnerable web app
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/) — free

### Practice Platforms
- [PortSwigger Academy labs](https://portswigger.net/web-security/all-labs) — free
- [PicoCTF](https://picoctf.org/) — free
- [TryHackMe](https://tryhackme.com/) — free rooms available
- [Hack The Box Academy](https://academy.hackthebox.com/) — free tier

### Recommended Books
- *The Web Application Hacker's Handbook* (Stuttard & Pinto) — commercial, check library access

### Mini Projects
- Directory brute-forcer
- HTTP header analyzer
- Subdomain finder
- Password auditor

### ✅ When am I ready to move on?
- [ ] I've completed at least the Apprentice-level labs on PortSwigger Academy
- [ ] I can explain and demonstrate SQL Injection, XSS, and CSRF
- [ ] I've solved several PicoCTF web challenges independently

---

## 08. Network Security

### Why should I learn this?
Web apps aren't the only attack surface. Understanding how to intercept, analyze, and attack network traffic is a core skill for both offensive and defensive security roles.

### What should I learn?
- Man-in-the-middle attacks
- ARP spoofing / poisoning
- Packet crafting and analysis
- Firewalls, IDS/IPS basics
- VPNs and how they actually protect traffic

### Free Resources
- [Wireshark](https://www.wireshark.org/) — free
- [TryHackMe — Network Security path (free rooms)](https://tryhackme.com/)

### Practice Platforms
- [TryHackMe](https://tryhackme.com/)
- [CyberDefenders](https://cyberdefenders.org/) — free blue-team labs
- [BlueTeamLabs Online](https://blueteamlabs.online/) — has free content

### Recommended Books
- *TCP/IP Illustrated* (W. Richard Stevens) — commercial, check library access

### Mini Projects
- Mini Intrusion Detection System (IDS)
- Packet analyzer / traffic logger
- ARP spoofing detector

### ✅ When am I ready to move on?
- [ ] I can capture and analyze suspicious traffic in Wireshark
- [ ] I understand how ARP spoofing enables a MITM attack
- [ ] I can explain the difference between an IDS and an IPS

---

## 09. Reverse Engineering

### Why should I learn this?
Reverse engineering is how you understand what a compiled program is *actually* doing — critical for malware analysis, exploit development, and understanding vulnerabilities at the binary level.

### What should I learn?
- Assembly basics (x86/x86-64)
- Disassemblers and debuggers
- Static vs dynamic analysis
- Basic binary exploitation concepts (buffer overflows, stack layout)

### Free Resources
- [OpenSecurityTraining](https://opensecuritytraining.info/) — free, in-depth courses on reverse engineering and exploitation
- [Malware Unicorn's RE101/RE102 workshops](https://malwareunicorn.org/#/workshops) — free, hands-on

### Practice Platforms
- [Crackmes.one](https://crackmes.one/) — free reverse engineering challenges of all difficulty levels

### Recommended Books
- *Hacking: The Art of Exploitation* (Jon Erickson) — commercial, check library access
- *Practical Malware Analysis* (Sikorski & Honig) — commercial, check library access

### Mini Projects
- Solve 5–10 beginner Crackmes
- Write up your solving process for one crackme as a blog post

### ✅ When am I ready to move on?
- [ ] I can read basic x86 assembly and understand what it's doing
- [ ] I've solved multiple beginner-level crackmes
- [ ] I understand how a stack-based buffer overflow overwrites the return address

---

## 10. Malware Analysis

### Why should I learn this?
Understanding how malware works — and how to analyze it safely — is core to defensive security (blue team, incident response) and deeply connected to everything you learned about operating systems and reverse engineering.

### What should I learn?
- Static analysis (strings, headers, imports)
- Dynamic analysis (sandboxing, behavior monitoring)
- Common malware techniques (persistence, obfuscation, C2 communication)
- Safe analysis environment setup (isolated VMs, snapshots)

### Free Resources
- [FLARE VM](https://github.com/mandiant/flare-vm) — free, a full malware analysis toolkit for Windows
- [REMnux](https://remnux.org/) — free Linux toolkit for malware analysis
- [ANY.RUN Community](https://any.run/) — free tier for interactive online malware sandboxing

### Practice Platforms
- Analyze samples from public malware research repositories in an **isolated, offline VM only** — never on your host machine

### Recommended Books
- *Practical Malware Analysis* (Sikorski & Honig) — commercial, check library access

### Mini Projects
- Set up your own isolated analysis lab (FLARE VM or REMnux)
- Write a static analysis report on a known, safe sample from a public malware research repository

### ✅ When am I ready to move on?
- [ ] I have a working isolated analysis environment set up
- [ ] I understand the difference between static and dynamic analysis
- [ ] I can identify basic persistence mechanisms in a sample report

---

## 11. Cryptography

### Why should I learn this?
Cryptography is behind almost everything you interact with securely — HTTPS, password storage, VPNs. You don't need to be a mathematician, but you need to understand what's actually happening instead of just "use AES" or "hash the password."

### What should I learn?
- Symmetric vs asymmetric encryption
- Hashing vs encryption (and why they're not the same thing)
- TLS/SSL handshake basics
- Common cryptographic mistakes (weak hashing, ECB mode, key reuse)

### Free Resources
- [Cryptopals Crypto Challenges](https://cryptopals.com/) — free, hands-on, widely respected in the security community
- [Khan Academy — Cryptography](https://www.khanacademy.org/computing/computer-science/cryptography) — free

### Practice Platforms
- [Cryptopals](https://cryptopals.com/) — work through the challenge sets

### Recommended Books
- *Serious Cryptography* (Jean-Philippe Aumasson) — commercial, check library access

### Mini Projects
- Implement a basic Caesar/Vigenère cipher cracker
- Work through the first Cryptopals challenge set

### ✅ When am I ready to move on?
- [ ] I can explain the difference between hashing and encryption
- [ ] I understand what a TLS handshake accomplishes
- [ ] I've completed at least Cryptopals Set 1

---

## 12. Cloud Security

### Why should I learn this?
Modern infrastructure runs on the cloud, and misconfigured cloud environments (open S3 buckets, overly permissive IAM roles) are one of the most common real-world breach causes today.

### What should I learn?
- IAM (Identity and Access Management) fundamentals
- Common misconfigurations (public storage buckets, exposed secrets)
- Shared responsibility model
- Cloud-native logging and monitoring basics

### Free Resources
- [AWS Skill Builder](https://skillbuilder.aws/) — free courses directly from AWS
- [Microsoft Learn](https://learn.microsoft.com/en-us/training/) — free, includes Azure security paths
- [Google Cloud Skills Boost](https://www.cloudskillsboost.google/) — has free introductory content

### Practice Platforms
- AWS Free Tier / Azure Free Account / Google Cloud Free Tier — practice directly, just watch your usage limits

### Recommended Books
- No single definitive free book — official cloud provider documentation (linked above) is the most current and free resource

### Mini Projects
- Deliberately misconfigure and then fix an S3 bucket in a free-tier AWS sandbox
- Write a script that audits IAM permissions for overly broad access

### ✅ When am I ready to move on?
- [ ] I understand the shared responsibility model
- [ ] I can identify a misconfigured storage bucket and explain the risk
- [ ] I've completed at least one free cloud security learning path

---

## 13. Active Directory

### Why should I learn this?
Active Directory runs the backbone of most corporate networks. A huge share of real-world enterprise penetration tests and red team engagements revolve entirely around AD misconfigurations and privilege escalation paths.

### What should I learn?
- AD structure: domains, forests, OUs, group policies
- Authentication protocols: Kerberos, NTLM
- Common attack paths: Kerberoasting, pass-the-hash, privilege escalation

### Free Resources
- [TryHackMe — Active Directory learning path (free rooms available)](https://tryhackme.com/)
- [Microsoft's Active Directory documentation](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/active-directory-domain-services) — free

### Practice Platforms
- [TryHackMe](https://tryhackme.com/) — several free AD-focused rooms
- [HackMyVM](https://hackmyvm.eu/) — some AD-focused machines

### Recommended Books
- No single definitive free book — hands-on labs (above) are the best free way to learn this topic

### Mini Projects
- Set up a small home lab AD environment (Windows Server free evaluation license + a client VM) and practice basic enumeration

### ✅ When am I ready to move on?
- [ ] I understand what Kerberoasting is and why it works
- [ ] I can explain the difference between NTLM and Kerberos authentication
- [ ] I've completed at least one free AD-focused room on TryHackMe

---

## 14. Mobile Security

### Why should I learn this?
Mobile apps are everywhere, and mobile security has its own quirks — different permission models, different storage mechanisms, different attack surfaces than web apps.

### What should I learn?
- Android app structure (APK, manifest, permissions)
- iOS app basics (IPA structure, sandboxing)
- Insecure data storage
- Common mobile app vulnerabilities (insecure communication, weak authentication)

### Free Resources
- [OWASP Mobile Application Security (MASTG/MASVS)](https://owasp.org/www-project-mobile-app-security/) — free, the standard reference

### Practice Platforms
- [OWASP MASTG hands-on crackmes](https://mas.owasp.org/crackmes/) — free

### Recommended Books
- No single definitive free book — the OWASP MASTG above functions as a complete free reference

### Mini Projects
- Decompile a simple test APK and review its manifest and permissions
- Find an intentionally insecure storage flaw in an OWASP MASTG crackme

### ✅ When am I ready to move on?
- [ ] I can decompile and inspect a basic APK
- [ ] I understand common insecure storage patterns on mobile
- [ ] I've solved at least one MASTG crackme

---

## 15. AI Security

### Why should I learn this?
This is where cybersecurity and AI meet. As more products get built on top of LLMs, a whole new attack surface has appeared — and most security professionals don't understand it deeply yet. Being fluent here puts you ahead.

### What should I learn?
- Prompt injection & jailbreaking
- Prompt leakage
- Model poisoning & adversarial ML basics
- LLM guardrails and secure RAG design
- AI red-teaming / pentesting methodology

### Free Resources
- [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/) — free
- [OWASP GenAI Security Project](https://genai.owasp.org/) — free
- [Garak](https://github.com/leondz/garak) — free, open-source LLM vulnerability scanner
- [Promptfoo](https://www.promptfoo.dev/) — free, open-source LLM testing/red-teaming tool
- [DeepTeam](https://github.com/confident-ai/deepteam) — free, open-source LLM red-teaming framework

### Practice Platforms
- Run Garak or Promptfoo against a local open-source model to see real prompt-injection results

### Recommended Books
- No dedicated book yet exists that stays current — this field moves fast, so the OWASP projects above are the best living references

### Mini Projects
- AI security scanner that tests a chatbot for common prompt-injection patterns
- AI-powered log analyzer for a SOC
- A guardrail layer sitting in front of an LLM API filtering unsafe outputs

### ✅ When am I ready to move on?
- [ ] I can successfully demonstrate a basic prompt injection against a test chatbot
- [ ] I understand what a "secure RAG" design has to defend against
- [ ] I've run an open-source LLM scanning tool (Garak/Promptfoo) at least once

---

## 16. CTF Platforms

Capture The Flag platforms are how you turn theory into muscle memory. Rotate between these depending on what you're currently studying.

- [PicoCTF](https://picoctf.org/) — free, beginner-friendly, great for fundamentals
- [Hack The Box Academy (Free Tier)](https://academy.hackthebox.com/) — free tier available
- [TryHackMe (Free Rooms)](https://tryhackme.com/) — many free rooms across every topic
- [OverTheWire](https://overthewire.org/wargames/) — completely free wargames
- [Root Me](https://www.root-me.org/) — free, huge variety of challenges

---

## 17. Practice Labs (Downloadable / Self-Hosted)

Run these on your own machine — no subscription needed.

- [VulnHub](https://www.vulnhub.com/) — free downloadable vulnerable VMs
- [HackMyVM](https://hackmyvm.eu/) — free vulnerable machines
- [Dockerlabs](https://dockerlabs.es/) — free Docker-based pentest labs
- [CyberDefenders](https://cyberdefenders.org/) — free blue-team-focused labs
- [BlueTeamLabs Online](https://blueteamlabs.online/) — free content available

---

## 18. Books

A short list, prioritizing free resources with commercial books noted as such (check library/university access before buying):

- *OSTEP* — free — pages.cs.wisc.edu/~remzi/OSTEP
- *The Linux Command Line* — free — linuxcommand.org
- *Eloquent JavaScript* — free — eloquentjavascript.net
- *The Web Application Hacker's Handbook* — commercial
- *Hacking: The Art of Exploitation* — commercial
- *Practical Malware Analysis* — commercial
- *The Shellcoder's Handbook* — commercial
- *Serious Cryptography* — commercial
- *Computer Networking: A Top-Down Approach* — commercial

---

## 19. YouTube Channels

- [Neso Academy](https://www.youtube.com/c/nesoacademy) — CS fundamentals
- [Professor Messer](https://www.youtube.com/user/professormesser) — networking & security certs
- [Abdul Bari](https://www.youtube.com/@abdul_bari) — data structures & algorithms
- [John Hammond](https://www.youtube.com/@_JohnHammond) — CTF walkthroughs and security concepts
- [LiveOverflow](https://www.youtube.com/@LiveOverflow) — binary exploitation, reverse engineering, deep dives

---

## 20. Career Tips

- **Build in public.** Push every project, every mini-tool, every writeup to GitHub with a clear README. This becomes your portfolio.
- **Write about what you learn.** A short blog post or GitHub writeup explaining a vulnerability you found or a concept you struggled with is worth more to employers than a certificate.
- **CTFs are practice, not the whole job.** Real work involves reporting, communication, and understanding business risk — practice writing clear, professional findings, not just capturing flags.
- **Pick a specialization eventually**, but not too early. Try web security, malware analysis, cloud security, and AI security before committing to one — you'll usually discover which one actually excites you rather than which one sounds impressive.
- **Certifications help get past HR filters**, but hands-on ability (shown through your GitHub and CTF profile) is what actually gets you hired and keeps you employed.

---

## ✅ Using this repo

Fork it, star it, and turn each section's checklist into your own tracker. Keep a `/projects` folder with a short README per finished project — that's what turns this from a reading list into a portfolio.

**Consistency beats intensity.**
