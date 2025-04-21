# Commands for Managing Groups and Permissions  

This section provides a detailed guide for managing groups and configuring permissions in Linux systems.

---

## 👥 1. Create a Group  

- **Create a Group Named `devteam`:**  
  `sudo groupadd devteam`  

---

## ➕ 2. Add Users to the Group  

- **Add `mark` to the Group:**  
  `sudo usermod -aG devteam mark`  

- **Add `elliot` to the Group:**  
  `sudo usermod -aG devteam elliot`  

---

## ✅ 3. Verify Group Membership  

- **Check if `mark` and `elliot` are in the Group:**  
  `groups mark`  
  `groups elliot`  

---

## 🔒 4. Change Permissions for the Group  

Example: Configure a directory `/project` to allow access for the `devteam` group.  

1. **Create the Directory:**  
   `sudo mkdir /project`  

2. **Change Group Ownership:**  
   `sudo chown :devteam /project`  

3. **Set Group Permissions:**  
   - Allow read, write, and execute for the group:  
     `sudo chmod 770 /project`  
   - **Permissions Breakdown:**  
     - **Owner:** Read, Write, Execute.  
     - **Group:** Read, Write, Execute.  
     - **Others:** No access.  

4. **Verify Permissions:**  
   `ls -ld /project`  
   - Expected output: `drwxrwx---`.  

---

## ⚙️ 5. Add Default Group Permissions  

- **Ensure All Files in `/project` Inherit the Group Permissions:**  
  `sudo chmod g+s /project`  

This command sets the **setgid** bit, ensuring that new files and directories created within `/project` automatically inherit the group ownership of `devteam`.  

---

These commands enable efficient group management and permissions configuration, ensuring proper access control and security in Linux environments.
