# Key Tools for Managing Users  

A summary of tools and methods for effectively managing local and domain user accounts across different operating systems.

---

## 🖥️ Windows  

### **Local Users:**  
- **Control Panel > User Accounts:**  
  A graphical interface to manage user accounts and settings.  
- **Computer Management > Local Users and Groups:**  
  Access advanced user management settings for creating, modifying, or deleting accounts.  

### **Domain Users:**  
- **Active Directory Users and Computers (ADUC):**  
  A centralized tool for managing domain accounts, permissions, and group memberships in Windows Server environments.  

---

## 🐧 Linux  

### **Local Users:**  
- Command-line tools for managing users:  
  - `useradd`: Creates new user accounts.  
  - `passwd`: Sets or updates user account passwords.  
  - `adduser`: A user-friendly script for adding accounts (varies by distribution).  

### **Domain Users:**  
- Integration with domain environments using:  
  - **LDAP (Lightweight Directory Access Protocol):** For directory-based authentication.  
  - **Kerberos:** A secure protocol for domain authentication.  
  - **Active Directory (via Samba/Winbind):** Allows Linux systems to join Windows domain environments and manage domain users.  
