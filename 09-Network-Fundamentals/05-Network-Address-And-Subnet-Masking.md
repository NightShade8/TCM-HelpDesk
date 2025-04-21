# Network Addresses and Subnet Masking

## 📄 Introduction to Network Addresses
**Network Address:** A unique identifier for devices in a network, enabling communication and data transfer.

**Key Points:**
- Used in both local and wide area networks (LANs and WANs).
- Composed of an IP address and a Subnet Mask.

## 🔢 IP Addresses
**Definition:** A numerical label assigned to devices in a network.

**Types:**
- **IPv4 (Internet Protocol Version 4):**
  - 32-bit address written as four octets (e.g., 192.168.1.1).
  - Example (binary representation): `11000000.10101000.00000001.00000001`.

- **IPv6 (Internet Protocol Version 6):**
  - 128-bit address written in hexadecimal (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
  - Larger address space for modern networks.

**Types of IPv4 Addresses:**
- **Public IP:** Globally unique; accessible over the Internet.
- **Private IP:** Used within local networks; ranges include:
  - `10.0.0.0 - 10.255.255.255`
  - `172.16.0.0 - 172.31.255.255`
  - `192.168.0.0 - 192.168.255.255`

## 🔗 Subnet Masks
**Definition:** A 32-bit number used to divide an IP address into the network and host portions.

**Format:** Written in the same dotted-decimal format as IPv4 (e.g., 255.255.255.0).

**Example:**
- **IP Address:** 192.168.1.100
- **Subnet Mask:** 255.255.255.0
  - **Network Portion:** 192.168.1
  - **Host Portion:** 100

## 🔢 CIDR (Classless Inter-Domain Routing) Notation
**Definition:** Shorthand for denoting subnet masks.

**Format:** Written as `IP/Prefix Length`.
- Example: `192.168.1.0/24`
  - **/24:** Indicates 24 bits are for the network, leaving 8 bits for hosts.

**Valid Examples:**
- Binary: `11111111.11111111.00000000.00000000` (Decimal: 255.255.0.0).

**Invalid Example:**
- Binary: `11111111.00000000.11111111.00000000` (Decimal: 255.0.255.0).

## 🖥️ Classes of IPv4 Addresses (Traditional)
| **Class** | **Range**                | **Default Subnet Mask** | **Usage**        |
|-----------|--------------------------|--------------------------|------------------|
| A         | 1.0.0.0 - 126.0.0.0     | 255.0.0.0 (/8)          | Large networks   |
| B         | 128.0.0.0 - 191.255.0.0 | 255.255.0.0 (/16)       | Medium networks  |
| C         | 192.0.0.0 - 223.255.255.0| 255.255.255.0 (/24)     | Small networks   |
| D         | 224.0.0.0 - 239.255.255.255| N/A                   | Multicast        |
| E         | 240.0.0.0 - 255.255.255.255| N/A                   | Experimental     |

## 🌍 Subnetting
**Purpose:** Divides a larger network into smaller, manageable sub-networks.

**Benefits:**
- Reduces network congestion.
- Improves security and performance.
- Efficiently utilizes IP addresses.

## 🧮 Subnet Mask and Host Calculation
**Formula:**
- **Number of Subnets:** `2^n`, where `n` is the number of borrowed bits.
- **Number of Hosts per Subnet:** `2^h - 2`, where `h` is the number of remaining host bits.

**Example:**
- **Subnet Mask:** 255.255.255.128 or /25.
- **Hosts:** `2^7 - 2 = 126`.

**Valid Octet Values:** `0, 128, 192, 224, 240, 248, 252, 254, 255`.

## 📊 Examples of Subnet Masks and CIDR
| **Subnet Mask**   | **CIDR** | **Number of Hosts** |
|--------------------|----------|---------------------|
| 255.255.255.0      | /24      | 254                 |
| 255.255.255.128    | /25      | 126                 |
| 255.255.255.192    | /26      | 62                  |

## 🌐 Broadcast and Network Addresses
- **Network Address:** The first address in a subnet (used to identify the subnet).
  - Example: `192.168.1.0/24`.
- **Broadcast Address:** The last address in a subnet (used to send data to all devices in the subnet).
  - Example: `192.168.1.255/24`.

## 📚 Summary
- **Network Address:** Identifies a network.
- **Subnet Mask:** Defines the network and host portions of an IP address.
- **Subnetting:** Crucial for efficient IP address utilization, enhanced security, and improved network management.
