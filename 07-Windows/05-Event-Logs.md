# Event Logs in Windows: Overview  

Event logs are essential for recording and analyzing significant system, security, and application-related events on a Windows computer. They aid in troubleshooting, monitoring, and auditing system behavior.

---

## 🗂️ Types of Event Logs  

1. **System Log:**  
   Contains events related to the operating system and its components.  
   Examples: Driver errors, hardware failures, and system shutdown/startup.  

2. **Application Log:**  
   Records events from applications or programs.  
   Examples: Application crashes and service-specific errors.  

3. **Security Log:**  
   Tracks security-related events like login attempts and privilege changes.  
   Examples: Successful/failed login attempts.  
   **Note:** Security logs follow configured audit policies.  

4. **Setup Log:**  
   Captures events during Windows installation or setup processes.  
   Useful for diagnosing installation-related issues.  

5. **Forwarded Events:**  
   Collects logs forwarded from other computers for centralized monitoring.  

---

## 🔍 Accessing Event Logs  

### **1. Using Event Viewer:**  
- Press `Win + R`, type `eventvwr`, and press Enter.  
- Navigate logs such as:  
  - **Windows Logs:** System, Application, Security, Setup, Forwarded Events.  
  - **Applications and Services Logs:** Logs specific to applications and services.  

### **2. Using Command Line or PowerShell:**  
- **Command Prompt:**  
  `wevtutil qe System` to query the system log.  
- **PowerShell:**  
  `Get-EventLog -LogName System` to view specific logs.  

---

## 📋 Event Log Structure  

Each log entry contains:  
- **Date/Time:** When the event occurred.  
- **Event ID:** Unique identifier for the event type.  
- **Source:** The component generating the event.  
- **Level:** Severity (e.g., Information, Warning, Error, Critical).  
- **User:** The user account under which the event occurred.  
- **Description:** Detailed information about the event.  

---

## 🔑 Common Event IDs  

| **Event ID** | **Log**       | **Description**                          |
|--------------|---------------|------------------------------------------|
| 4624         | Security      | Successful logon.                        |
| 4625         | Security      | Failed logon attempt.                    |
| 6008         | System        | Unexpected shutdown.                     |
| 1000         | Application   | Application crash or error.              |
| 41           | System        | Kernel power issue (e.g., crash-related).|

---

## 🛠️ Managing Event Logs  

1. **Filter Events:**  
   Use **Filter Current Log** in Event Viewer to narrow down by Event ID, severity, source, etc.  

2. **Export Logs:**  
   Right-click a log (e.g., System) and select **Save All Events As** to export logs in `.evtx`, `.txt`, or `.xml` formats.  

3. **Clear Logs:**  
   Clear old logs by right-clicking a log (e.g., Application) and selecting **Clear Log**.  

4. **Enable/Disable Logging:**  
   Use **Group Policies** or **Audit Policies** to manage specific types of logging, especially security logs.  

---

## 📈 Use Cases for Event Logs  

- **Troubleshooting:** Diagnose application or system errors.  
- **Security Monitoring:** Detect unauthorized access attempts and monitor malicious activity.  
- **Compliance:** Ensure regulatory adherence by auditing events.  
- **Performance Monitoring:** Identify resource bottlenecks to optimize performance.  

---

## 🏁 Conclusion  

Event logs are invaluable for managing Windows systems. Understanding their structure and types enables effective troubleshooting, security monitoring, and performance optimization.  
