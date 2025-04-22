# 🖥️ Active Directory Management

## 📋 User Management
### **Creating a New User**
```
Powershell:
New-ADUser -Name "John Doe" -SamAccountName jdoe -UserPrincipalName jdoe@company.local -Path "OU=Users,DC=company,DC=local" -AccountPassword (ConvertTo-SecureString "Password123" -AsPlainText -Force) -Enabled $true
```
####Disabling A User Account
```powershell
Disable-ADAccount -Identity jdoe
```
####Resettting a User Password
```powershell
Set-ADAccountPassword -Identity jdoe -Reset -NewPassword (ConvertTo-SecureString "NewPass123" -AsPlainText -Force)```
####Group Management
**Creating a New Group**
```powershell
New-ADGroup -Name "IT Support" -GroupScope Global -Path "OU=Groups,DC=Company,DC=local"
```

###📋 Computer Management
#### **Listing All Computers in AD**
```powershell
Get-ADComputer -Filter *
```
**Joining a Computer to a Domain (Run on the Client Machine)**
```powershell
Add-Computer -DomainNAme "Company.local" -Credential "company\\admin"
```

###📚 Summary
Active Directory management ensures efficient control over users, groups, and devices, improving security and access control.
