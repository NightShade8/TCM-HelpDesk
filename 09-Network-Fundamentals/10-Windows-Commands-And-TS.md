# **Windows Network Commands & Troubleshooting**

## 📄 Basic Network Commands

These commands help in viewing and managing network settings in Windows.

| **Command**            | **Description**                                                                 |
|------------------------|---------------------------------------------------------------------------------|
| `ipconfig`             | Displays IP configuration details of all network adapters.                      |
| `ipconfig /all`        | Shows detailed network adapter information, including MAC address & DNS.        |
| `ipconfig /release`    | Releases the current IP address assigned by DHCP.                               |
| `ipconfig /renew`      | Requests a new IP address from the DHCP server.                                 |
| `ipconfig /flushdns`   | Clears the DNS cache to resolve domain-related issues.                          |

---

## 🔄 Connectivity & Troubleshooting Commands

Used to diagnose network connectivity and performance.

| **Command**             | **Description**                                                                 |
|--------------------------|--------------------------------------------------------------------------------|
| `ping <IP/Domain>`       | Sends test packets to check if a host is reachable.                            |
| `ping -t <IP>`           | Continuously pings a target until manually stopped.                            |
| `tracert <IP/Domain>`    | Shows the route packets take to reach a destination.                           |
| `pathping <IP/Domain>`   | Combines `ping` and `tracert`, providing detailed network path analysis.       |
| `nslookup <Domain>`      | Queries DNS servers for IP address resolution of a domain.                     |
| `netstat -an`            | Displays active network connections and listening ports.                       |

---

## 🖧 Managing Network Connections

Useful for managing and configuring network interfaces.

| **Command**                                      | **Description**                                                     |
|--------------------------------------------------|---------------------------------------------------------------------|
| `netsh interface show interface` 				   | Lists all network interfaces.                                       |
| `netsh wlan show profiles`      				   | Displays saved Wi-Fi network profiles.                              |
| `netsh wlan show profile <Wi-Fi_Name> key=clear` | Reveals stored Wi-Fi password.   					                 |
| `netsh int ip reset`       				       | Resets TCP/IP stack to fix network issues.                          |
| `netsh winsock reset`          				   | Resets Windows network socket settings.                             |

---

## 🔐 Firewall & Port Commands

For managing Windows Firewall and checking network security.

| **Command**                                                                                | **Description**                                                     |
|--------------------------------------------------------------------------------------------|---------------------------------------------------------------------|
| `netsh advfirewall show allprofiles`                       							     | Displays firewall settings for all profiles                         |
| `netsh advfirewall firewall add rule name="AllowPing" protocol=ICMPv4 dir=in action=allow` | Allows ping requests through the firewall                           |
| `telnet <IP> <Port>`                                    								     | Tests if a port is open on a remote machine (requires Telnet client)|

---

## 📶 Wi-Fi & Network Adapter Commands

Used to diagnose and manage network adapters.

| **Command**                  | **Description**                                                     |
|------------------------------|---------------------------------------------------------------------|
| `netsh wlan show interfaces` | Displays Wi-Fi connection details.                                  |
| `netsh wlan disconnect`      | Disconnects from the current Wi-Fi network.                         |
| `getmac`                     | Displays the MAC address of all network adapters.                   |
| `arp -a`                     | Shows the ARP table (IP-to-MAC mappings).                           |

---

## 📚 Summary

- **`ipconfig` & `ping`:** Diagnose connectivity issues.
- **`tracert` & `pathping`:** Identify slow network paths.
- **`nslookup`:** Resolve domain names to IPs.
- **`netstat` & `telnet`:** Check active connections & open ports.
- **`netsh`:** Manage network settings, Wi-Fi, firewall, and reset configurations.
