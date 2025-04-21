# Notes on Ports in Networking

## 📄 What Are Ports?

- A **port** is a logical communication endpoint used to differentiate network services running on a device.
- Ports work with **IP addresses** to direct traffic to the correct application.
- They operate at **Layer 4 (Transport Layer)** of the **OSI Model**.
- Two main protocols use ports:
  - **TCP (Transmission Control Protocol):** Reliable, connection-oriented.
  - **UDP (User Datagram Protocol):** Fast, connectionless.

---

## 🔢 Port Number Ranges

| **Range**           | **Description**           			                                                     |
|---------------------|------------------------------------------------------------------------------------------|
| **0 – 1023**        | **Well-Known Ports:** Reserved for system and popular services (e.g., HTTP, HTTPS, FTP). |
| **1024 – 49151**    | **Registered Ports:** Used by software vendors for specific applications.  				 |
| **49152 – 65535**   | **Dynamic/Ephemeral Ports:** Temporarily assigned to client applications.  				 |

---

## 🔗 Commonly Used Ports

| **Service**                  | **Protocol**     | **Port Number** |
|------------------------------|------------------|-----------------|
| HTTP (Web)        		   | TCP              | 80              |
| HTTPS (Secure Web) 		   | TCP              | 443             |
| FTP (File Transfer)  		   | TCP              | 20, 21          |
| SSH (Secure Shell) 		   | TCP              | 22              |
| Telnet (Remote Access)       | TCP              | 23              |
| SMTP (Email Sending)         | TCP              | 25              |
| DNS (Domain Name System)     | UDP/TCP          | 53              |
| DHCP (IP Address Assignment) | UDP    	  	  | 67, 68          |
| POP3 (Email Retrieval)       | TCP              | 110             |
| IMAP (Email Retrieval)	   | TCP              | 143             |
| RDP (Remote Desktop) 		   | TCP              | 3389            |
| MySQL Database        	   | TCP              | 3306            |

---

## 🔄 How Ports Work in Communication

1. **Client Requests a Service:** A client device sends a request using a specific **destination port** (e.g., HTTP on port 80).
2. **Server Listens on the Port:** The server listens for incoming connections on that port and responds accordingly.
3. **Response Sent Back to Client:** The server sends data back using a temporary **ephemeral port** for the client.

---

## 🛡️ Port Security & Management

- **Firewalls:** Block or allow traffic based on port numbers.
- **Port Scanning:** Tools like `nmap` scan open ports for security testing.
- **Closing Unused Ports:** Prevents unauthorized access to network services.

---

## 📚 Summary

- **Ports** help direct network traffic to the right application/service.
- Divided into three ranges: **well-known, registered, and dynamic.**
- **Common protocols** (HTTP, FTP, SSH, etc.) use specific port numbers.
- **Firewalls and security tools** manage and monitor ports to prevent attacks.
