# 🐧 Essential Linux Commands Reference

A comprehensive guide to the most common Linux terminal commands.

---

## 📂 File & Directory Navigation
| Command | Description |
| :--- | :--- |
| ⁠ pwd ⁠ | *Print **Working **D*irectory (Shows your current path) |
| ⁠ ls -la ⁠ | *L*ist all files, including hidden ones, with details |
| ⁠ cd <dir> ⁠ | *Change **D*irectory |
| ⁠ cd .. ⁠ | Move up one directory level |
| ⁠ mkdir <name> ⁠ | Create a new directory |

---

## 📄 File Operations
| Command | Description |
| :--- | :--- |
| ⁠ touch <file> ⁠ | Create a new empty file |
| ⁠ cp <src> <dest> ⁠ | *Cop*y a file (⁠ -r ⁠ for directories) |
| ⁠ mv <src> <dest> ⁠ | *Move or **rename* a file/directory |
| ⁠ rm <file> ⁠ | *Rem*ove a file |
| ⁠ rm -rf <dir> ⁠ | *Recursively and **f*orcefully remove a directory (Caution!) |
| ⁠ cat <file> ⁠ | Display entire file content |
| ⁠ head -n 5 <file> ⁠| View first 5 lines of a file |
| ⁠ tail -f <file> ⁠ | Follow a file in real-time (great for logs) |

---

## 🛡️ Permissions & Ownership
Permissions are calculated as: *Read (4) + Write (2) + Execute (1)*.

•⁠  ⁠⁠ sudo <command> ⁠: Run command with root privileges.
•⁠  ⁠⁠ chmod 755 <file> ⁠: Set permissions to ⁠ rwxr-xr-x ⁠.
•⁠  ⁠⁠ chown user:group <file> ⁠: Change file owner and group.

---

## ⚙️ System Information
•⁠  ⁠⁠ top ⁠ or ⁠ htop ⁠: Monitor CPU, RAM, and running processes.
•⁠  ⁠⁠ df -h ⁠: Check *disk **f*ree space in human-readable format.
•⁠  ⁠⁠ free -m ⁠: Check RAM usage in Megabytes.
•⁠  ⁠⁠ uname -a ⁠: Display kernel and system info.
•⁠  ⁠⁠ uptime ⁠: See how long the system has been running.

---

## 🔍 Searching & Filtering
•⁠  ⁠⁠ grep "pattern" <file> ⁠: Search for text inside a file.
•⁠  ⁠⁠ find . -name "*.log" ⁠: Find files by name in the current directory.
•⁠  ⁠⁠ history ⁠: Show list of previously executed commands.
•⁠  ⁠⁠ command | grep "search" ⁠: Filter the output of a command.

---

## 🌐 Networking
•⁠  ⁠⁠ ip addr ⁠: Show IP addresses and network interfaces.
•⁠  ⁠⁠ ping <host> ⁠: Check connectivity to a host (e.g., google.com).
•⁠  ⁠⁠ curl -O <url> ⁠: Download a file from a URL.
•⁠  ⁠⁠ ssh user@host ⁠: Connect to a remote server.

---

## 💡 Keyboard Shortcuts
•⁠  ⁠⁠ Tab ⁠: Auto-complete file or directory names.
•⁠  ⁠⁠ Ctrl + C ⁠: Stop the currently running command.
•⁠  ⁠⁠ Ctrl + L ⁠: Clear the terminal screen.
•⁠  ⁠⁠ Ctrl + R ⁠: Search through your command history.
*
