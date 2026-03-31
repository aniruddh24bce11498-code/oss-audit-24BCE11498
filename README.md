[README.md](https://github.com/user-attachments/files/26381679/README.md)
# Open Source Audit — Git

![Bash](https://img.shields.io/badge/Shell-Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Git](https://img.shields.io/badge/Software-Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/OS-Ubuntu_WSL-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![License](https://img.shields.io/badge/License-GPL_v2-blue?style=flat-square&logo=gnu&logoColor=white)

A structured audit of **Git**. This project includes a written report and five Bash shell scripts that demonstrate practical Linux system administration skills.

---

## Student Info

| Field | Details |
|---|---|
| **Name** | Aniruddh gupta |
| **Reg. No.** | 24BCE11498 |
| **Course** | Open Source Software (Linux Administration) — CSE0002 |
| **Chosen Software** | Git — GPL v2 |
| **GitHub** | Duke-07 |

---

## About Git

Git is a free and open-source **distributed version control system** created by **Linus Torvalds in 2005**. It was built after the Linux kernel community lost access to their proprietary tool (BitKeeper), and Torvalds wrote it from scratch in just a few weeks.

Unlike older centralized systems like CVS or Subversion, Git gives every developer a complete copy of the repository including its full history. This allows offline work, faster operations, and no single point of failure. Today, Git is the backbone of modern software development and powers platforms like GitHub and GitLab.

---

## License — GPL v2

Git is released under the **GNU General Public License version 2 (GPL v2)** — a *copyleft* license that grants users four core freedoms:

| Freedom | Description |
|---------|-------------|
| Freedom 0 | Run the program for any purpose |
| Freedom 1 | Study and modify the source code |
| Freedom 2 | Redistribute copies freely |
| Freedom 3 | Distribute modified versions |

**Copyleft condition:** Any distributed modification of Git must also be released under GPL v2, ensuring the software and its improvements stay open permanently. This is the key difference from permissive licenses like MIT, where modifications can be closed off.

---

## Repository Structure

```
Duke-07 / Linux-Shell-Scripting-Audit-System-Analysis-with-Open-Source-Tools
│
├── Project Screenshots/
│   ├── 1.jpeg                # Script 1 terminal output
│   ├── 2.jpeg                # Script 2 terminal output
│   ├── 3.jpeg                # Script 3 terminal output
│   ├── 4.jpeg                # Script 4 terminal output
│   └── 5.jpeg                # Script 5 terminal output
│
├── CaseStudy.pdf             # Written case study report
├── OSS Capstone Project File.pdf   # Full capstone project report
│
├── Script1.sh                # System Identity Report
├── Script2.sh                # FOSS Package Inspector
├── Script3.sh                # Disk & Permission Auditor
├── Script4.sh                # Log File Analyzer
└── Script5.sh                # Open Source Manifesto Generator
```

---

## Scripts Overview

### Script 1 — System Identity Report
Displays system information including username, kernel version, Linux distribution, uptime, and current date/time.  
**Concepts used:** Variables, `uname`, `whoami`, `uptime`, `lsb_release`, `echo`

### Script 2 — FOSS Package Inspector
Checks whether `git` is installed, shows package details via `dpkg`, displays the installed version, and prints a philosophy note using a `case` statement.  
**Concepts used:** `if-then-else`, `case` statement, `dpkg -l`, pipe with `grep`

### Script 3 — Disk & Permission Auditor
Loops through five key system directories and reports permissions, owner, and size for each. Also checks for the Git configuration directory.  
**Concepts used:** `for` loop, `ls -ld`, `du -sh`, `awk`, `cut`

### Script 4 — Log File Analyzer
Accepts a filename and optional keyword (default: `error`) as arguments, checks if the file exists, counts keyword occurrences, and shows the last 5 matching lines.  
**Concepts used:** `while read` loop, `if-then`, counter variables, `$1`/`$2` arguments, `grep`, `tail`

### Script 5 — Open Source Manifesto Generator
Asks the user three questions and generates a personalized open-source manifesto, saving it to a `.txt` file and printing it on screen.  
**Concepts used:** `read -p`, string interpolation, file redirection (`>`, `>>`), `date`, `cat`

---

## How to Run

**Prerequisites:** Ubuntu Linux or WSL, Bash shell, Git installed

```bash
# Clone the repository
git clone https://github.com/Duke-07/Linux-Shell-Scripting-Audit-System-Analysis-with-Open-Source-Tools.git
cd Linux-Shell-Scripting-Audit-System-Analysis-with-Open-Source-Tools

# Make all scripts executable
chmod +x Script*.sh

# Run scripts
./Script1.sh
./Script2.sh
./Script3.sh
./Script4.sh /var/log/syslog error
./Script5.sh
```

---

## Script Outputs

### Script 1 — System Identity Report
![Script 1 Output](./Project%20Screenshots/1.jpeg)

### Script 2 — FOSS Package Inspector
![Script 2 Output](./Project%20Screenshots/2.jpeg)

### Script 3 — Disk & Permission Auditor
![Script 3 Output](./Project%20Screenshots/3.jpeg)

### Script 4 — Log File Analyzer
![Script 4 Output](./Project%20Screenshots/4.jpeg)

### Script 5 — Open Source Manifesto Generator
![Script 5 Output](./Project%20Screenshots/5.jpeg)

---

## Tools & Environment

| Tool | Purpose |
|---|---|
| Ubuntu Linux (WSL) | Operating system |
| Bash | Shell scripting |
| Nano | Script editor |
| Git | Version control |
| dpkg / grep / awk | Package inspection and text processing |

---

## Objectives

- Understand the concept and philosophy of open-source software
- Learn basic Linux commands and Bash shell scripting
- Automate system-level tasks using shell scripts
- Analyze files and directories using Linux utilities
- Audit a real open-source project across origin, license, ethics, and ecosystem

---
