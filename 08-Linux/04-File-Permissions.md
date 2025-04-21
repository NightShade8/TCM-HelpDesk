# File Permissions Overview  

A guide to understanding and managing file permissions in Linux systems.

---

## 🔒 Permission Structure  

- **Format:**  
  Permissions are displayed as `rwxrwxrwx`, representing **Owner**, **Group**, and **Others**.  
  - **`r` (Read):** Value `4` - Allows viewing contents.  
  - **`w` (Write):** Value `2` - Allows modifying contents.  
  - **`x` (Execute):** Value `1` - Allows running the file as a program.  

---

## 📋 Check Permissions  

- Use the `ls -l [file]` command to display file permissions.  
  Example outputs:  
  - **`rw-r--r--`:**  
    - **Owner:** `rw-` (read, write).  
    - **Group:** `r--` (read-only).  
    - **Others:** `r--` (read-only).  

---

## 🔄 Changing Permissions  

### **1. Using `chmod` Command**  

#### **Symbolic Mode:**  
- **Add Permission:**  
  `chmod u+x file` (adds execute for the user).  
  Example: `chmod u+x test.txt`.  

- **Remove Permission:**  
  `chmod g-w file` (removes write for group).  
  Example: `chmod g-w test.txt`.  

- **Set Permission:**  
  `chmod o=r file` (sets read-only for others).  

#### **Numeric Mode (Octal):**  
- Set using numeric values:  
  - `chmod 755 file`:  
    - `7` (Owner): `rwx`.  
    - `5` (Group): `r-x`.  
    - `5` (Others): `r-x`.  

---

### **2. Change Ownership (`chown`)**  

- **Change File Owner:**  
  `chown user file`.  
  Example: `chown kali test.txt`.  

- **Change Owner and Group:**  
  `chown user:group file`.  
  Example: `chown kali:root test.txt`.  

---

### **3. Change Group (`chgrp`)**  

- Change the group ownership:  
  `chgrp group file`.  
  Example: `sudo chgrp root test.txt` (changes group to root).  

---

## 💡 Common Examples  

- **Make a Script Executable:**  
  `chmod +x script.sh`.  

- **Full Access to Owner, Read-Only for Others:**  
  `chmod 744 file.txt`.  

---

These commands are foundational for managing file access and ensuring proper administration in Linux systems.
