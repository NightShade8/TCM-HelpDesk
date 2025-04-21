# Routers

## 📄 What is a Router?

- A **Router** is a networking device that connects multiple networks and directs data packets between them.
- It determines the best path for forwarding data across networks using IP (Internet Protocol) addresses.
- Operates at **Layer 3 (Network Layer)** of the **OSI Model**.

---

## 🔄 Functions of a Router

1. **Packet Forwarding**: Routes data packets to their destination network based on IP addressing.
2. **Network Address Translation (NAT):**
   - Translates private IP addresses to a public IP for Internet communication.
3. **Traffic Control**: Manages traffic between networks, ensuring efficient data flow.
4. **Firewall Features:**
   - Can filter traffic for security by blocking or allowing specific packets.
5. **Dynamic Routing:**
   - Uses protocols (e.g., OSPF, BGP, RIP) to dynamically adapt to changes in the network.

---

## 🖧 How Routers Work

1. **Receives a Packet**: The router inspects the packet's destination IP address.
2. **Looks Up Routing Table**: Determines the best path to the destination network.
3. **Forwards the Packet**: Sends the packet to the next router or device in the path.

---

## 🔌 Types of Routers

1. **Home/Small Office Routers**:
   - Used for personal or small business networks.
   - Combines features like Wi-Fi access and NAT.
2. **Enterprise Routers**:
   - Used in large organizations.
   - Supports advanced routing, multiple connections, and security features.
3. **Core Routers**:
   - Operate in the backbone of the Internet.
   - High-speed, designed to handle large data volumes.
4. **Edge Routers**:
   - Connect internal networks to external networks (e.g., ISPs).
5. **Virtual Routers**:
   - Software-based routers that run on virtual machines.

---

## 🔄 Static vs. Dynamic Routing

- **Static Routing**:
   - Manually configured routes.
   - Suitable for small networks.
   - No adaptability to network changes.

- **Dynamic Routing**:
   - Uses protocols (e.g., OSPF, RIP, BGP) to update routes automatically.
   - Adapts to changes in the network topology.

---

## 🌐 Common Routing Protocols

| **Protocol** | **Abbreviation**       | **Type**          | **Key Features**                      |
|--------------|-------------------------|-------------------|---------------------------------------|
| RIP          | Routing Information Protocol | Distance Vector | Simple, low overhead, slow convergence. |
| OSPF         | Open Shortest Path First | Link-State       | Faster convergence, scalable.         |
| BGP          | Border Gateway Protocol | Path-Vector      | Used for Internet routing.            |

---

## 🔑 Key Terms

- **Routing Table**: A database in the router that holds information about the routes to different networks.
- **Gateway**: The device/router that acts as an entry/exit point for a network.
- **Default Route**: A fallback route used when no specific route is found in the routing table.

---

## ⚙️ Router Features

- **QoS (Quality of Service)**: Prioritizes certain types of network traffic.
- **DHCP (Dynamic Host Configuration Protocol)**: Assigns IP addresses to devices automatically.
- **VPN (Virtual Private Network)**: Securely connects networks over the Internet.

---

## 📚 Summary

- A router connects and manages communication between multiple networks.
- Uses IP addressing to determine the best path for data packets.
- Supports both static and dynamic routing to adapt to network needs.
- Key to network efficiency, scalability, and security.
