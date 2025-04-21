# Short Notes on Updating and Upgrading in Kali Linux  

A guide to the basic commands and best practices for managing updates and upgrades in Kali Linux.

---

## Update and Upgrade Basics  
1. **Update:**
Fetches the Lates list of Available software and their versions from repositories
```
sudo apt update
```
2. **Upgrade:**
	Installs the latest version of software packages excluding kernel and major system changes
```
sudo apt upgrade
```
3. **Full Upgrade**
	Updates all packages, including kernel updates and system-level changes.
```
sudo apt full-upgrade
```
## 🔧 Common Combined Usage

- Run Update and Upgrade in one step:
	`sudo apt update && sudo apt upgrade -y`
- Run a full upgrade in one step
	`sudo apt update && sudo apt full-upgrade -y`
---
## 🧹 Clean Up After Upgrading

1. Remove Unnecessary Packages:

```
sudo apt autoremove
```

2. Clear Downloaded Package Cache:

```
sudo apt clean
```

---
## ✅ Best Practices 
- Always run `sudo apt update` before upgrading
- Use `sudo apt full-upgrade` cautiously as it may replace or remove system packages
- Regularly check for updates to keep your system secure and functional

