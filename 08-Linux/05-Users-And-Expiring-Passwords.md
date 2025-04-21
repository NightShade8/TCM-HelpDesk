# Commands for Adding Users and Expiring Passwords  

This section outlines essential commands for managing user accounts and setting password expiration policies in Linux systems.

---

## 👤 1. Adding Users  

Commands to create new user accounts:  
- **Add User `mark`:**  
  `sudo adduser mark`  
  - Follow the prompts to set a password and user details.  

- **Add User `elliot`:**  
  `sudo adduser elliot`  
  - Similarly, set a password for `elliot`.  

---

## 🔒 2. Expiring Passwords  

Force users to reset their passwords upon next login:  
- **Expire `mark`'s Password:**  
  `sudo passwd -e mark`  

- **Expire `elliot`'s Password:**  
  `sudo passwd -e elliot`  

---

## ✅ 3. Verify Expiry Status  

Check the password expiry settings for user accounts:  
- **View `mark`'s Expiry Status:**  
  `sudo chage -l mark`  

- **View `elliot`'s Expiry Status:**  
  `sudo chage -l elliot`  

---

## 📅 Additional Notes  

Set specific expiry dates for user accounts:  
- **Expire Account on February 1, 2025:**  
  `sudo chage -E 2025-02-01 mark`  
  `sudo chage -E 2025-02-01 elliot`  

This command ensures the user accounts expire on a predefined date.  

---

These commands are vital for securely managing user access and enforcing password policies within Linux environments.
