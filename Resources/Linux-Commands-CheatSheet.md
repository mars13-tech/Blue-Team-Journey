# Linux Commands for Blue Team

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

[Continue with more commands you learned]
