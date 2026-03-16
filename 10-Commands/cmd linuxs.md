Here is a comprehensive Linux Command Cheat Sheet in Markdown format. You can copy this block and save it as a .md file (e.g., linux_commands.md).
🐧 Linux Command Cheat Sheet
📂 File & Directory Navigation
Command	Description
ls	List files and directories in the current folder
ls -la	List all files, including hidden ones, with details
cd [dir]	Change directory to [dir]
cd ..	Move up one directory level
pwd	Show the full path of the current directory
mkdir [name]	Create a new directory
📄 File Operations
Command	Description
touch [file]	Create an empty file
cat [file]	Display the contents of a file
less [file]	View a file with pagination (press q to exit)
cp [src] [dest]	Copy a file or directory
mv [src] [dest]	Move or rename a file or directory
rm [file]	Delete a file
rm -r [dir]	Delete a directory and its contents recursively
🛡️ Permissions & Ownership
Command	Description
chmod [mode] [file]	Change file permissions (e.g., chmod 755 script.sh)
chown [user]:[group] [file]	Change file owner and group
sudo [command]	Run a command with root/admin privileges
⚙️ System Information & Management
Command	Description
top	Display real-time running processes
htop	Interactive process viewer (requires installation)
df -h	Show free disk space in human-readable format
free -m	Show RAM usage in MB
uname -a	Show system and kernel information
history	View a list of recently used commands
🌐 Networking
Command	Description
ping [host]	Check connectivity to a host (e.g., ping google.com)
ip addr	Show all network interfaces and IP addresses
curl [URL]	Download content or interact with an API
ssh [user]@[host]	Connect to a remote machine via SSH
🔍 Searching & Filtering
Command	Description
grep "[pattern]" [file]	Search for a string inside a file
find [path] -name [name]	Search for files by name
locate [file]	Quickly find a file's path (uses a database)
