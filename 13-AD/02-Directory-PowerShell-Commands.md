# 🏢 Active Directory PowerShell Commands

## 📌 PowerShell for Active Directory
PowerShell provides powerful command-line tools for managing **Active Directory** objects efficiently.

✅ **Key Benefits:**
- Automation of repetitive tasks
- Bulk management of users and groups
- Advanced filtering and reporting

---

## 🛠️ User Management Commands

### **Create a New User**
```powershell
New-ADUser -Name "John Doe" -SamAccountName jdoe -UserPrincipalName jdoe@company.local -Path "OU=Users,DC=company,DC=local" -AccountPassword (ConvertTo-SecureString "Password123" -AsPlainText -Force) -Enabled $true
```

### **Disable a User Account**
```powershell
Disable-ADAccount -Identity jdoe
```

### **Reset a User Password**
```powershell
Set-ADAccountPassword -Identity jdoe -Reset -NewPassword (ConvertTo-SecureString "NewPass123" -AsPlainText -Force)
```

### **Get All Users**
```powershell
Get-ADUser -Filter *
```

---

## 🔄 Group Management Commands

### **Create a New Group**
```powershell
New-ADGroup -Name "IT Support" -GroupScope Global -Path "OU=Groups,DC=company,DC=local"
```

### **Add a User to a Group**
```powershell
Add-ADGroupMember -Identity "IT Support" -Members jdoe
```

---

## 💻 Computer Management Commands

### **List All Computers**
```powershell
Get-ADComputer -Filter *
```

### **Join Computer to Domain**
```powershell
Add-Computer -DomainName "company.local" -Credential "company\admin"
```

---

## 📝 Sample User Creation Script

```powershell
# Import Active Directory Module
Import-Module ActiveDirectory

# Prompt for user details
$FirstName = Read-Host "Enter First Name"
$LastName = Read-Host "Enter Last Name"
$Username = Read-Host "Enter Username"
$Password = Read-Host "Enter Password" -AsSecureString

# Set user details
$DisplayName = "$FirstName $LastName"
$OU = "OU=Users,DC=company,DC=local"
$UPN = "$Username@company.local"
$SAM = $Username

# Create new AD User
New-ADUser `
    -GivenName $FirstName `
    -Surname $LastName `
    -Name $DisplayName `
    -UserPrincipalName $UPN `
    -SamAccountName $SAM `
    -Path $OU `
    -AccountPassword $Password `
    -Enabled $true `
    -ChangePasswordAtLogon $true

Write-Host "User $DisplayName ($Username) has been created successfully!" -ForegroundColor Green
```

---

## 🔒 Security Commands

### **Force Group Policy Update**
```powershell
gpupdate /force
```

### **Check Domain Controller Status**
```powershell
dcdiag /v
```

### **Check Replication Status**
```powershell
repadmin /replsummary
```

---

## 📚 Summary
PowerShell commands make Active Directory management more **efficient**, **scriptable**, and **consistent** across your organization.
