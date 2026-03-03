# Day 2 - March 2, 2026 - Blue Team Fundamentals & Linux Basics

## ⏱️ Time Spent: 5 hours

## ✅ Tasks Completed
- [x] Kali Linux VM fully operational
- [x] Cisco Introduction to Cybersecurity - Module 1 & 2
- [x] TryHackMe: "Intro to Defensive Security"
- [x] TryHackMe: "Careers in Cyber"
- [x] TryHackMe: "Linux Fundamentals Part 1"
- [x] Practiced 15+ Linux commands in Kali terminal
- [x] Created Linux command cheat sheet
- [x] Updated GitHub repository
- [x] LinkedIn post published

---

## 📚 Cisco - Introduction to Cybersecurity

### Module 1: The Need for Cybersecurity

**Why Cybersecurity Matters:**
- Organizations face constant cyber threats
- Data breaches can cost millions and damage reputation
- Cybersecurity protects confidentiality, integrity, and availability (CIA Triad)
- Every device connected to internet is a potential target

**Common Cyber Threats:**
- Malware (viruses, trojans, ransomware)
- Phishing attacks
- Denial of Service (DoS)
- Data breaches
- Insider threats

**Cybersecurity Domains:**
- Network Security
- Application Security
- Information Security
- Operational Security
- Disaster Recovery

**Blue Team Role:**
- Defend systems and networks
- Monitor for threats
- Respond to incidents
- Maintain security controls

### Module 2: Attacks, Concepts and Techniques

**Types of Attacks:**
1. **Social Engineering** - Manipulating people to reveal information
2. **Malware** - Malicious software designed to damage/gain access
3. **Network Attacks** - Exploiting network vulnerabilities
4. **Wireless Attacks** - Targeting WiFi and wireless protocols
5. **Web-based Attacks** - SQL injection, XSS, CSRF

**Attack Vectors:**
- Email attachments
- Malicious websites
- USB drives
- Vulnerable software
- Weak passwords

**Defense Strategies:**
- Firewalls
- Intrusion Detection Systems (IDS)
- Antivirus software
- Security awareness training
- Patch management
- Access controls

**Security Controls:**
- **Preventive** - Stop attacks before they happen
- **Detective** - Identify attacks in progress
- **Corrective** - Fix damage after attack
- **Deterrent** - Discourage attackers

---

## 🛡️ TryHackMe - Intro to Defensive Security

### What is Defensive Security?
Defensive security focuses on preventing intrusions and detecting/responding to threats. Unlike offensive security (ethical hacking), blue team members defend the infrastructure.

### Security Operations Center (SOC)

**What is a SOC?**
A team of cybersecurity professionals who monitor networks and systems 24/7 to detect and respond to security incidents.

**SOC Analyst Responsibilities:**
- Monitor security alerts from SIEM
- Investigate suspicious activities
- Analyze logs to identify threats
- Respond to security incidents
- Create incident reports
- Threat hunting
- Tune detection rules to reduce false positives

**SOC Tiers:**
- **Tier 1 (Junior/Alert Analyst):** Monitor alerts, triage incidents, escalate to Tier 2
- **Tier 2 (Incident Responder):** Deep investigation, containment, coordinate response
- **Tier 3 (Threat Hunter/SME):** Advanced threat hunting, malware analysis, tool development

### Digital Forensics and Incident Response (DFIR)

**Digital Forensics:**
- Collecting and analyzing digital evidence
- File system analysis
- Memory forensics
- Network forensics
- Timeline reconstruction

**Incident Response Process:**
1. Preparation
2. Identification
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

### Malware Analysis
- **Static Analysis:** Examine without executing
- **Dynamic Analysis:** Execute in controlled environment (sandbox)
- Understanding malware behavior to improve defenses

---

## 💼 TryHackMe - Careers in Cyber

### Blue Team Career Paths

**1. Security Analyst / SOC Analyst**
- Monitor security systems
- Analyze alerts and logs
- Entry-level role (target: 12-18 LPA)
- Skills: SIEM, log analysis, networking

**2. Incident Responder**
- Handle security breaches
- Forensic investigation
- Mid-level role
- Skills: Forensics, IR process, malware analysis

**3. Threat Hunter**
- Proactively search for threats
- Advanced role
- Skills: MITRE ATT&CK, scripting, deep log analysis

**4. Security Engineer**
- Build/maintain security tools
- Automation and integration
- Skills: Programming, cloud security, DevSecOps

**5. Digital Forensics Investigator**
- Deep dive investigations
- Evidence collection
- Skills: Forensic tools, legal procedures, reporting

**6. Malware Analyst**
- Reverse engineer malware
- Develop signatures/detections
- Skills: Assembly, debugging, sandboxing

**My Target Role:** SOC Analyst Tier 1 → Goal is 15 LPA within 6 months

**Skills Needed for SOC Analyst:**
- SIEM platforms (Splunk, ELK)
- Log analysis
- Network fundamentals
- Incident response basics
- Scripting (Python, Bash)
- Security frameworks (MITRE ATT&CK, Cyber Kill Chain)

---

## 🐧 TryHackMe - Linux Fundamentals Part 1

### Why Linux Matters for Blue Team
- Most servers run Linux
- All SIEM/security tools have Linux versions
- System logs are in Linux format
- Command line is essential for investigations

### Linux Commands Learned & Practiced

#### Navigation Commands
| Command | Description | Example | Use Case |
|---------|-------------|---------|----------|
| `pwd` | Print working directory | `pwd` → `/home/kali` | Know where you are |
| `ls` | List files/directories | `ls -la` | See all files including hidden |
| `cd` | Change directory | `cd /var/log` | Navigate to logs folder |
| `cd ~` | Go to home directory | `cd ~` | Quick return home |
| `cd ..` | Go up one level | `cd ..` | Navigate back |

#### File Operations
| Command | Description | Example | Use Case |
|---------|-------------|---------|----------|
| `cat` | Display file contents | `cat file.txt` | View entire file |
| `head` | Show first 10 lines | `head -n 20 file.txt` | Preview file start |
| `tail` | Show last 10 lines | `tail -n 50 /var/log/syslog` | View recent logs |
| `tail -f` | Follow file in real-time | `tail -f /var/log/auth.log` | Monitor live logs |
| `less` | View file page by page | `less largefile.txt` | Read large files |
| `grep` | Search in files | `grep "error" syslog` | Find specific patterns |
| `wc` | Word/line count | `wc -l file.txt` | Count log entries |

#### File/Directory Management
| Command | Description | Example | Use Case |
|---------|-------------|---------|----------|
| `touch` | Create empty file | `touch newfile.txt` | Create placeholder |
| `mkdir` | Create directory | `mkdir evidence` | Organize files |
| `cp` | Copy files | `cp log.txt backup.txt` | Backup evidence |
| `mv` | Move/rename files | `mv old.txt new.txt` | Organize investigation |
| `rm` | Remove files | `rm tempfile.txt` | Clean up |
| `rm -r` | Remove directory | `rm -r folder/` | Delete folder |

#### System Information
| Command | Description | Example | Use Case |
|---------|-------------|---------|----------|
| `whoami` | Current username | `whoami` → `kali` | Verify user context |
| `hostname` | Computer name | `hostname` | Identify system |
| `uname -a` | System information | `uname -a` | OS details |
| `date` | Current date/time | `date` | Timestamp investigations |
| `uptime` | System uptime | `uptime` | Check last reboot |
| `history` | Command history | `history` | Review actions taken |

#### Finding & Searching
| Command | Description | Example | Use Case |
|---------|-------------|---------|----------|
| `find` | Find files | `find / -name "*.log" 2>/dev/null` | Locate log files |
| `locate` | Quick file search | `locate syslog` | Fast file finding |
| `which` | Find program location | `which nmap` | Verify tool installation |

#### Pipes and Redirection
| Command | Description | Example | Use Case |
|---------|-------------|---------|----------|
| `\|` (pipe) | Send output to next command | `cat file.txt \| grep "error"` | Chain commands |
| `>` | Redirect output (overwrite) | `echo "test" > file.txt` | Save output |
| `>>` | Redirect output (append) | `echo "test2" >> file.txt` | Add to file |
| `2>/dev/null` | Suppress errors | `find / -name test 2>/dev/null` | Clean output |

### Important Directories for Blue Team

| Directory | Purpose | Why It Matters |
|-----------|---------|----------------|
| `/var/log/` | System logs | **CRITICAL** - All security events logged here |
| `/var/log/auth.log` | Authentication logs | Failed logins, sudo usage |
| `/var/log/syslog` | System messages | General system events |
| `/etc/` | Configuration files | See how services are configured |
| `/etc/passwd` | User accounts | List all users on system |
| `/etc/shadow` | Password hashes | Actual password storage |
| `/home/` | User directories | User files and activities |
| `/tmp/` | Temporary files | Malware often hides here |
| `/var/` | Variable data | Logs, caches, databases |

### Commands Practiced in Kali VM Today

```bash
# Checked my location
pwd

# Listed all files including hidden
ls -la

# Navigated to logs directory
cd /var/log

# Viewed authentication logs (login attempts)
cat auth.log

# Searched for failed login attempts
grep "Failed password" auth.log

# Counted failed login attempts
grep "Failed password" auth.log | wc -l

# Viewed last 20 lines of syslog
tail -n 20 syslog

# Created practice directory
mkdir ~/BlueTeam-Practice
cd ~/BlueTeam-Practice

# Created test file
echo "This is a security log entry" > testlog.txt

# Appended more data
echo "Another log entry" >> testlog.txt

# Viewed the file
cat testlog.txt

# Searched for pattern
grep "security" testlog.txt

# Viewed system users
cat /etc/passwd

# Searched for my user
grep "kali" /etc/passwd

# Checked command history
history | tail -n 20
