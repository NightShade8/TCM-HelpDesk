# 🏢 Active Directory in Windows Server 2022

## 📌 What is Active Directory?
Active Directory (AD) in **Windows Server 2022** is a centralized directory service that manages **users, computers, groups, and security policies** within a network.

✅ **Key Functions:**
- Authentication & Authorization
- Resource Management
- Domain Environment Control

---

## 🛠️ Setting Up Active Directory

### **1️⃣ Install AD Domain Services**
- Open **Server Manager** → **Add Roles and Features**
- Select **Active Directory Domain Services**
- Complete installation

### **2️⃣ Promote Server to Domain Controller**
- Select **"Add a new forest"** and enter domain name
- Set **DSRM password**
- Review settings and install
- Server will reboot with AD DS active

---

## 👤 User and Group Management

### **User Management**
- Open **Active Directory Users and Computers (ADUC)**
- Navigate to target **OU**
- Create users with login credentials
- Set password policies

### **Group Management**
- Create **Security** or **Distribution** groups
- Set **Group Scope**: Global, Domain Local, or Universal
- Add members to groups

---

## 🖥️ Computer and OU Management

### **Joining a Computer to Domain**
- On client computer: System → About → Rename this PC
- Enter domain name and admin credentials
- Restart to apply changes

### **Creating Organizational Units**
- In ADUC: Right-click domain → New → OU
- Name and organize OUs by department or function

---

## 🔐 Group Policy Management

- Open **Group Policy Management**
- Create and name GPOs
- Configure policies for security and settings
- Link GPOs to OUs or domains

---

## 📊 Maintenance & Monitoring

- Check DC status: `dcdiag /v`
- Check replication: `repadmin /replsummary`
- Force Group Policy update: `gpupdate /force`
- Back up AD using Windows Server Backup

---

## 🔒 Best Practices

✔ Use structured **OUs** for better management
✔ Enforce strong **password policies**
✔ Limit **administrative privileges**
✔ Keep DCs **updated and patched**
✔ Implement **account lockout policies**
✔ Use multiple DCs for **redundancy**

---

## 📚 Summary
Active Directory on **Windows Server 2022** provides robust **user and resource management** through centralized authentication and policy enforcement.
