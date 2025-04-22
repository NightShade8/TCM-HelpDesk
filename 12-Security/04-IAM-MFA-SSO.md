# 🔑 IAM, MFA, and SSO

## 📄 What is Identity and Access Management (IAM)?

**Identity and Access Management (IAM)** ensures that the right individuals have appropriate access to resources in an organization. It protects systems and data from unauthorized access by managing **user identities, authentication, and authorization**.

---

## 🛠️ Key Components of IAM

- **Identity Management** – Handles user account creation, updates, and deletion.
- **Access Control** – Ensures users have appropriate permissions based on their roles.
- **Authentication** – Verifies user identity using passwords, biometrics, or Multi-Factor Authentication (MFA).
- **Authorization** – Grants access based on predefined rules and policies.
- **Auditing & Monitoring** – Tracks user activities and access logs for security compliance.

✅ **Benefits of IAM**
- Enhances security by preventing unauthorized access.
- Reduces insider threats.
- Improves compliance with regulations like **GDPR, HIPAA, ISO 27001**.
- Supports **Role-Based Access Control (RBAC)** and **Least Privilege Principle**.

🛠 **Examples of IAM Solutions**
- Microsoft Entra ID (Azure AD)
- Okta
- AWS IAM
- Google Cloud IAM

---

## 🔒 Multi-Factor Authentication (MFA)

**Multi-Factor Authentication (MFA)** adds an extra layer of security by requiring users to verify their identity using multiple authentication factors.

### **Types of Authentication Factors**
1️⃣ **Something You Know** – Passwords, PINs, security questions.  
2️⃣ **Something You Have** – OTPs, smart cards, security keys.  
3️⃣ **Something You Are** – Biometrics like fingerprint or face recognition.

✅ **Benefits of MFA**
- Strengthens security beyond traditional passwords.
- Prevents phishing and credential theft.
- Meets compliance requirements (e.g., PCI-DSS, NIST, GDPR).

🛠 **Examples of MFA Solutions**
- Google Authenticator, Microsoft Authenticator
- Duo Security
- YubiKey (Hardware MFA)

---

## 🌍 Single Sign-On (SSO)

**Single Sign-On (SSO)** allows users to log in once and gain access to multiple applications without needing to enter credentials again.

### **How SSO Works**
1️⃣ User logs in with a single credential.  
2️⃣ SSO system verifies identity and issues a **session token**.  
3️⃣ The token is used for authentication across various services.

✅ **Benefits of SSO**
- **Convenience** – Eliminates multiple login requirements.
- **Improved Security** – Reduces password fatigue.
- **Reduced IT Workload** – Fewer password reset requests.
- **Enhanced User Experience** – Seamless access to applications.

### **Common SSO Protocols**
- **OAuth 2.0** – Secure authorization for web and mobile apps.
- **SAML (Security Assertion Markup Language)** – Used in enterprise authentication.
- **OpenID Connect (OIDC)** – Extends OAuth 2.0 for identity verification.

🛠 **Examples of SSO Providers**
- Microsoft Entra ID (Azure AD SSO)
- Okta SSO
- Google Workspace SSO
- OneLogin

---

## 📚 Summary

IAM, MFA, and SSO **enhance security, streamline access management, and prevent unauthorized access**.  
- **IAM manages user identities and permissions**.  
- **MFA strengthens authentication security**.  
- **SSO simplifies authentication across multiple services**.  

A well-implemented IAM strategy with **MFA and SSO** significantly improves **security posture and user experience**.
