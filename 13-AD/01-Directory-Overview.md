# 🏢 Active Directory (AD) Overview

## 📌 What is Active Directory?
Active Directory (AD) is a **directory service** developed by **Microsoft** for Windows domain networks. It manages **users, computers, and resources** within an organization. 

✅ **Key Functions:**
- Authentication & Authorization
- Centralized User & Resource Management
- Group Policies Enforcement

---

## 🛠️ Key Components of Active Directory

### **1️⃣ Domain Controller (DC)**
- Stores the AD database and handles authentication.
- Enforces security policies.

### **2️⃣ Active Directory Database (NTDS.dit)**
- Contains **user accounts, groups, computers**, and policies.

### **3️⃣ Objects**
- **Users** – Individual accounts.
- **Groups** – Collections of users with specific permissions.
- **Computers** – Devices within the domain.

### **4️⃣ Domains**
- Logical group of AD objects.
- Example: `company.local`.

### **5️⃣ Organizational Units (OUs)**
- Structures AD objects for easier management.
- Helps apply **Group Policies (GPOs)**.

### **6️⃣ Group Policy Objects (GPOs)**
- A set of rules and settings applied across the domain.
- Used for security, software deployment, and configurations.

### **7️⃣ Trusts**
- Allows cross-domain authentication.
- Types: **One-way trust, Two-way trust, Forest trust**.

---

## 🔍 How Active Directory Works

1️⃣ **User logs in** → Credentials are sent to the **Domain Controller**.  
2️⃣ **DC authenticates** using the **AD database**.  
3️⃣ **If successful**, user accesses authorized resources.  
4️⃣ **Group Policies (GPOs)** are applied based on **OU and group membership**.

---

## ⚡ Benefits of Active Directory

✔ **Centralized Management** – Control all users and policies from one place.
✔ **Security & Authentication** – Ensures proper verification.
✔ **Scalability** – Works for small to large networks.
✔ **Group Policies** – Enforce security settings across devices.
✔ **Single Sign-On (SSO)** – One authentication for multiple services.

---

## 📚 Summary
Active Directory **simplifies IT management**, enhances **security**, and ensures **efficient authentication** across an organization. 🚀
