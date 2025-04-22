# 🛠️ Key Components of Active Directory

## 🖥️ Domain Controller (DC)
- **Primary server** that runs AD, authenticating users and enforcing security policies.
- Stores the **AD database** for users, computers, and permissions.

## 📂 Active Directory Database (NTDS.dit)
- Contains **user accounts, groups, computers**, and policies.
- Replicated across **Domain Controllers** for redundancy.

## 🔗 Objects
- **Users** – Individual accounts for employees.
- **Groups** – Collections of users with shared permissions.
- **Computers** – Devices connected to the domain.
- **Printers & Resources** – Shared devices in the network.

## 🌎 Domains
- Logical grouping of **users, computers, and resources** under a common security boundary.
- Example: `company.local`.

## 🏢 Organizational Units (OUs)
- Used to structure **users, groups, and computers** for easier management.
- Helps apply **Group Policies (GPOs)** efficiently.

## ⚙️ Group Policy Objects (GPOs)
- **Rules and settings** applied to users and computers within a domain.
- Used for **security configurations, software deployment, and system restrictions**.

## 🔄 Trusts
- Allow different domains or forests to share authentication resources securely.
- Types: **One-way trust, Two-way trust, Forest trust**.

## 📚 Summary
Active Directory components ensure **structured management, security enforcement, and resource allocation** within a domain environment.
