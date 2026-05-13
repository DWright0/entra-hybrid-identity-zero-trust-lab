# 🔐 Entra ID Hybrid Identity + Zero Trust Lab

## 📌 Overview

This project simulates a real-world **Zero Trust Identity Security implementation** using Microsoft Entra ID (Azure AD).

The lab demonstrates:

- Conditional Access policy design
- Identity Protection (Sign-in Risk + User Risk)
- MFA enforcement
- Forced password reset for compromised users
- Real authentication flows and validation through logs

---

## 🧱 Environment

- Microsoft Entra ID (Azure AD)
- Conditional Access Policies
- Identity Protection (P2 Features)
- Microsoft Authenticator (MFA)
- Test Users + Security Groups

---

## 🧩 Architecture

- Test users assigned to a **Zero Trust security group**
- Policies applied at group level (not tenant-wide)
- Risk-based authentication decisions
- Real login simulations using browser + mobile device

---

# 🛠️ 1. Overview

### Conditional Access Policies Dashboard
![Policies Dashboard](screenshots/01-overview/policies-dashboard.png)

### Zero Trust Test Group
![Test Group](screenshots/01-overview/test-group.png)

---

# ⚙️ 2. Policy Configuration

## Conditional Access Overview
![Overview](screenshots/02-policy-config/conditional-access-overview.png)

## Group Targeting (Zero Trust Scope)
![Group Targeting](screenshots/02-policy-config/group-targeting.png)

## Policies Enabled
![Policies Enabled](screenshots/02-policy-config/policies-enabled.png)

---

## 🔐 Sign-in Risk Policy (MFA)

### Condition Configuration
![Sign-in Risk Condition](screenshots/02-policy-config/signin-risk-condition.png)

### Grant Control (Require MFA)
![Sign-in Risk Grant](screenshots/02-policy-config/signin-risk-grant.png)

### Policy Overview
![Sign-in Risk Overview](screenshots/02-policy-config/signin-risk-mfa-overview.png)

---

## ⚠️ User Risk Policy (Password Reset)

### Condition Configuration
![User Risk Condition](screenshots/02-policy-config/user-risk-condition.png)

### Grant Control (Password Change)
![User Risk Grant](screenshots/02-policy-config/user-risk-grant.png)

---

## 🔐 3. Policy Enforcement (Real Authentication Flow)

### MFA Challenge Triggered
![MFA Challenge](screenshots/03-enforcement/mfa-challenge-triggered.png)
=======
### Policy Overview
![User Risk Overview](screenshots/02-policy-config/user-risk-overview.png)


---

# 🔒 3. Policy Enforcement (Real Authentication Flow)

## MFA Challenge Triggered
![MFA Challenge](screenshots/03-enforcement/mfa-challenge-triggered.png)

## MFA Registration Required
![MFA Registration](screenshots/03-enforcement/mfa-registration.png)

## MFA After Authentication
![MFA After](screenshots/03-enforcement/mfa-challenge-after-registration.png)


### MFA After Authentication
![MFA After](screenshots/03-enforcement/mfa-challenge-after-registration.png)

---

### Password Change Enforcement
=======
## Password Change Enforcement

![Password Change](screenshots/03-enforcement/password-change-enforced.png)

## Successful Login
![Successful Login](screenshots/03-enforcement/successful-login.png)

---

# 📊 4. Logging & Validation

## Sign-in Logs
![Sign-in Logs](screenshots/04-logs/signin-logs.png)

## Conditional Access Policy Evaluation
![Policy Evaluation](screenshots/04-logs/policy-evaluation.png)

---

# 🧠 Key Takeaways

- Zero Trust requires **verification at every access attempt**
- Policies should be applied using **groups for scalability**
- Identity Protection enables **risk-based decisions**
- MFA is critical but must be combined with:
  - Risk signals
  - Conditional access logic
- Logs are essential for validating security posture

---

# 🚀 Skills Demonstrated

- Microsoft Entra ID (Azure AD)
- Conditional Access Policy Design
- Identity Protection (User Risk / Sign-in Risk)
- MFA Implementation
- Authentication Flow Analysis
- Security Logging & Troubleshooting
- Zero Trust Architecture Concepts

---

# 🎯 Outcome

This lab simulates how modern organizations:

- Detect risky sign-ins
- Enforce MFA dynamically
- Force credential resets for compromised users
- Validate enforcement through real authentication logs

---

# 📌 Next Steps

- Integrate with AWS (IAM + Federation)
- Deploy infrastructure using Terraform
- Add monitoring (CloudWatch / Sentinel)
- Expand into full Cloud Security architecture
