# 🔐 Active Directory Security Best Practices

## 🛡 Essential Security Measures

✔ **Enable Multi-Factor Authentication (MFA)** to protect logins.  
✔ **Use Group Policies (GPOs)** to enforce security settings.  
✔ **Limit Administrative Privileges** to reduce risks.  
✔ **Enable Auditing & Logging** to track changes and detect suspicious activity.  
✔ **Regularly Update and Patch** domain controllers to prevent vulnerabilities.  
✔ **Implement Account Lockout Policies** to prevent brute force attacks.  

---

## 🛠 Monitoring & Auditing

### **Check Domain Controller Health**
```powershell
dcdiag /v
```

### **Check Replication Between Domain Controllers**
```powershell
repadmin /replsummary
```

### **Force a Group Policy Update on Clients**
```powershell
gpudate /force
```

### **Monitor Login Attempts**
```powershell
Get-EventLog -LogName Security | Where-Object{$_.EventID -eq 4625}

## **📚 Summary**
Active directory security requires MFA, auditing, enforcing GPOs, restricting privileges, and continuous monitoring to prevent cyber threats. 
