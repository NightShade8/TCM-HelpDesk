# 🧑‍💻 Local vs. Domain Users – Summary

### 🖥️ Local Users
- Created on and limited to a single machine.
- Managed locally via Control Panel (Windows) or `useradd` (Linux).
- No access to domain or network-wide resources unless configured.
- Common in standalone setups and personal devices.

### 🏢 Domain Users
- Managed by a domain controller (e.g., Active Directory).
- Can log in to any domain-connected device with proper permissions.
- Access to shared resources and group policies.
- Suitable for enterprises and large networks.

### 🔍 Comparison Table
| Feature             | Local Users           | Domain Users                   |
|---------------------|------------------------|--------------------------------|
| Scope               | Local machine only     | Domain-wide                    |
| Authentication      | Stored locally         | Via domain controller          |
| Resource Access     | Local resources        | Network-wide resources         |
| Management          | On-device              | Centralized via domain tools   |
| Offline Availability| Always                 | Cached credentials possible    |
| Common Use          | Home/standalone PCs    | Businesses, schools, orgs      |

### 🔄 Hybrid Use Cases
- Devices often include both types.
- IT uses local admin accounts for recovery; users use domain credentials for access.

### 🛠️ Management Tools
- **Windows**: Control Panel, Computer Management, Active Directory Users & Computers.
- **Linux**: `useradd`, LDAP, Kerberos, Winbind.

---

# 📋 Windows Event Logs – Summary

### 🗂️ Log Types
- **System**: OS-related events (drivers, hardware).
- **Application**: App errors or logs.
- **Security**: Auth events like logons, audit trails.
- **Setup**: Installation-related events.
- **Forwarded Events**: Logs from other systems.

### 🧭 Access Methods
- **GUI**: `eventvwr` (Event Viewer).
- **CLI**: `wevtutil`, `Get-EventLog` in PowerShell.

### 📑 Event Structure
- Includes: Timestamp, Event ID, Source, Severity, User, Description.

### 🔢 Common Event IDs
| ID    | Type      | Description                     |
|-------|-----------|---------------------------------|
| 4624  | Security  | Successful login                |
| 4625  | Security  | Failed login                    |
| 6008  | System    | Unexpected shutdown             |
| 1000  | App       | App crash/error                 |
| 41    | System    | Kernel power error              |

### ⚙️ Management Features
- Filter, export, clear logs.
- Customize with Audit Policies or GPO.

### 📈 Use Cases
- Troubleshooting issues.
- Monitoring user activity and security.
- Ensuring compliance and diagnostics.

---

# 💻 Windows 10 CMD Essentials – Summary

### 📂 Navigation
- `dir`, `cd`, `cls`, `tree`: Browse and clean screen.

### 📁 File Ops
- `mkdir`, `rmdir`, `del`, `copy`, `move`, `rename`: Manage folders/files.

### 🧠 System Diagnostics
- `ipconfig`, `ping`, `systeminfo`, `tasklist`, `taskkill`, `shutdown`: Diagnose or control system.

### 💾 Disk Tools
- `chkdsk`, `diskpart`, `format`: Storage repair/partitioning.

### 🔍 Search Utilities
- `find`, `where`: Locate strings or executables.

### 👤 User/Admin Commands
- `net user`, `netstat`, `whoami`: Manage users and sessions.

### 🧰 Utility Tools
- `echo`, `type`, `fc`, `set`, `help`: Display, compare, and configure.

### 🧩 Advanced Tools
- `sfc`, `powershell`, `reg`, `wmic`: Repair system or access system internals.

### ⚡ Tips & Tricks
- `Ctrl + C`: Cancel command.
- `Tab`: Autocomplete.
- `>`: Redirect output (e.g., `dir > out.txt`).

---
