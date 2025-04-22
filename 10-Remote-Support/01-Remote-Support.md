# 🧰 Remote Support & SSH Using OpenSSH Overview
A summarized reference guide for understanding remote support fundamentals, common tools, secure access using OpenSSH, and troubleshooting techniques.

---

## 🔍 **Remote Support Overview**
Explains the concept of remote support and how IT assistance can be provided remotely.

### 🌟 **How Remote Support Works**
- Establish a remote session using specialized software.
- Users may need to grant permission for technicians to access their systems.
- Technicians can view, control, and configure the remote device as needed.

---

## 🧱 **Common Remote Support Tools**
Summarizes key tools used for remote assistance.

| **Tool** | **Features** |
| --- | --- |
| **TeamViewer** | Secure, cross-platform, easy file sharing. |
| **AnyDesk** | Lightweight, fast, good for low-bandwidth connections. |
| **Microsoft Remote Desktop (RDP)** | Built-in for Windows, best for internal network access. |
| **Chrome Remote Desktop** | Simple, browser-based, requires Google account. |
| **LogMeIn** | Enterprise-grade, supports unattended access. |
| **Splashtop** | Secure and optimized for business IT support. |

---

## ⚡ **Types of Remote Support**
Describes different ways remote support can be provided.

1. **Unattended Access** – Technicians can access the system anytime without user approval.
2. **Attended Support** – The user must be present to approve and assist during the session.

---

## 🔐 **Security Considerations for Remote Support**
Lists essential security practices.

🔒 **Use Strong Authentication** – Require passwords, 2FA, or company login.

🔒 **Encrypt Connections** – Ensure remote software uses **end-to-end encryption**.

🔒 **Log and Monitor Sessions** – Track access history for security purposes.

🔒 **User Consent Required** – The user must approve before accessing sensitive data.

🔒 **Limit Access** – Restrict access to specific systems or functions.

---

## 🛠 **Troubleshooting Common Remote Support Issues**
Identifies common problems and solutions.

| **Issue** | **Solution** |
| --- | --- |
| Unable to connect | Check **internet connection** on both ends. |
| Software blocked | Ensure **firewall & antivirus** allow remote access. |
| Lag or slow response | Use a **wired connection** and close unused apps. |
| Permission denied | Ensure **user grants access** and has admin rights. |
| Session disconnects | Check for **network stability** and reconnect. |

---

# 🧰 SSH Using OpenSSH Overview
A summarized reference guide for managing secure remote access using OpenSSH.

---

## 🔍 **What is OpenSSH?**
Explains OpenSSH as a suite of tools for **secure remote access, authentication, and file transfers**.

### 🌟 **Key Features**
- **Open-source implementation** of SSH protocol.
- **Supports Linux, macOS, and Windows**.
- **Uses default port 22**.

---

## 🧱 **Installing OpenSSH**
Instructions for setting up OpenSSH on different systems.

### 🖥️ **Linux (Debian/Ubuntu-based)**
```bash
sudo apt update && sudo apt install openssh-server -y
```
### 🖥️ Linux (RHEL/CentOS-based)
```
sudo tum install openssh-server -y
```
### 🖥️ Windows (PowerShell - Admin Mode)
```
Add-WindowsFeature -name OpenSSH-Server
```
### 🛠 Managing SSH Service
Common Commands to Control OpenSSH Service:
```
sudo systemctl start ssh #Start the SSH Service

sudo systemctl stop ssh # Stop the SSH Service

sudo systemctl restart ssh # Restart SSH Service After Changes.

sudo systemctl enable ssh #Enable SSH to Start on boot

sudo systemctl status ssh #Check SSh Service Status
```
###🔐 SSH Authentication Methods
Explains password-based and key-based authentication.

###⚡ Password Authentication (Less Secure)
Default method, but vulnerable to brute-force attacks.

###⚡ Key-Based Authentication (Recommended)
1. Generate SSH Key Pair (Client Machine)
```
ssh-keygen -t rsa -b 4096
```
2. Copy Public Key to Remote Server
```
ssh-copy-id user@remote_host
```
3. Login Withouth Password
```
ssh user@remote_host
```

### 🚀 Transferring Files Using SSH
Uses SCP and SFTP for secure file transfers. 

### 📦 Secure Copy Protocol (SCP)
```
scp file.txt user@remote_host:/path/ #Copy file to remote system

scp -r folder/ user@remote_host:/path/ # Copy Folder Recursively 

scp user@remote_host:/path/file.txt #Download file from remote system
```

### 🌐 Secure File Transfer Protocol (SFTP)
```
sft user@remote_host

ls # list files on remote system

get file.txt #Download File

put file.txt #Upload file

exit #exit sftp session
```

### ⚡ Securing OpenSSH
- Best Practices for Secure SSH Connections. 
####🔒 Change Default SSH Port Edit /etc/ssh/sshd_config:
```
Port 2222
```
Restart SSH:
```
sudo systemctl restart ssh
```
Disable Root Login
```
PermitRootLogin no
```
Limit Access to Specific Users
```
AllowUsers alice bob
```
Enable Firewall for SSH
```
sudo ufw allow 22/tcp
```
For a Custom Port:
```
sudo ufw allow 2222/tcp
```

### 🛠 Troubleshooting OpenSSH Issues
Common Problems and Solutions
```
Connection refused #Ensure SSH service is running (sudo systemctl start ssh)

Permission Denied (PublicKey) # verify key is in ~/.ssh/authorized_keys

Slow login #Disable DNS Lookup in sshd_config (UseDNS no)

Host Key Verification Failed #Remove old key: ssh-keyegn -R remote_host
```

###📚 Summary
- Remote Support allows IT Techs to assit users globally
- Security Practices such as encryption and limited access improve safety
- OpenSSH provides secure remote access, file transfers, and tunnelling
- Key-based authentication is recommended for enhanced security
- Port forwarding allows tunneling of network connections

