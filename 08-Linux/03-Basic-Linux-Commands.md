# Basic Linux Commands  

A comprehensive guide to essential Linux commands for managing files, directories, processes, and system resources.  

---

## 📁 File and Directory Management  

- **`ls`:** List files and directories.  
  Example: `ls -l` (detailed view).  

- **`cd [path]`:** Change directory.  
  Example: `cd /home/user`.  

- **`pwd`:** Print the current directory.  

- **`mkdir [dir]`:** Create a directory.  
  Example: `mkdir new_folder`.  

- **`rmdir [dir]`:** Remove an empty directory.  

- **`rm [file/dir]`:** Remove files or directories.  
  Example: `rm -r folder` (delete folder recursively).  

- **`cp [src] [dest]`:** Copy files/directories.  
  Example: `cp file.txt /backup/`.  

- **`mv [src] [dest]`:** Move or rename files/directories.  
  Example: `mv oldname.txt newname.txt`.  

---

## 📄 File Viewing and Editing  

- **`cat [file]`:** Display file contents.  

- **`nano [file]`:** Edit a file using the nano editor.  

- **`less [file]`:** View file contents page by page.  

- **`head [file]`:** Display the first 10 lines of a file.  

- **`tail [file]`:** Display the last 10 lines of a file.  
  Example: `tail -f logfile` (follow updates in real-time).  

---

## 🔒 File Permissions and Ownership  

- **`chmod [mode] [file]`:** Change file permissions.  
  Example: `chmod 755 script.sh`.  

- **`chown [user:group] [file]`:** Change ownership of a file.  
  Example: `chown user:group file.txt`.  

---

## 🖥️ System Information  

- **`uname -a`:** Display system information.  

- **`df -h`:** Show disk usage in human-readable format.  

- **`du -sh [dir]`:** Show size of a directory.  

- **`free -h`:** Display memory usage.  

- **`top`:** Show running processes.  

- **`htop`:** Interactive process viewer (if installed).  

- **`uptime`:** Show system uptime.  

---

## 🔄 Process Management  

- **`ps`:** Display running processes.  

- **`kill [PID]`:** Terminate a process by its PID.  
  Example: `kill -9 1234` (force terminate).  

- **`jobs`:** Show background jobs.  

- **`bg`:** Resume a job in the background.  

- **`fg`:** Bring a job to the foreground.  

---

## 🌐 Networking  

- **`ping [host]`:** Check network connectivity.  

- **`ifconfig` / `ip a`:** Display network interfaces.  

- **`curl [URL]`:** Transfer data from a URL.  

- **`wget [URL]`:** Download files from a URL.  

- **`netstat -tul
