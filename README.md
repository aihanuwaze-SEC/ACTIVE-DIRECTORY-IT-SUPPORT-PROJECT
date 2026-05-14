# Active Directory IT Support Project

## Overview
This project demonstrates foundational Active Directory skills used in IT support roles. It focuses on user account management, group-based access control, and troubleshooting common issues in a Windows environment.

This project reinforces prior experience supporting users and systems by applying Active Directory concepts in a hands-on lab environment.

---

## Tools & Environment
- Windows Virtual Machine
- Active Directory concepts
- Command Prompt
- TryHackMe platform

## Active Directory Console
![ADUC](Screenshots./Active-directory-users-and-computer-console.png)

---
## Organizational Unit (OU) Management
### Scenario: Creating an OU for interns
- created a new organizational unit (OU) to organize user accounts
- demonstrated how OUs help structure domain environments
![Create OU](Screenshots./create-OU-interns.png)

### Scenario: Cleaningup users in OU
- Reviewed user accounts within the Sales Organizational unit
- Identified unnecessary or inactive users
- Removed two users to maintain proper accesss control

**Before Cleanup:**
![Before Cleanup](Screenshots./sales-OU-users-before-cleanup.png)

**After Cleanup**
![After Cleanup](Screenshots./sales-OU-users-after-cleanup.png)

### Scenario: Remooving Deprecated Department (R&D OU)
-Identified an outdated organizational unit following company restructuring
-Removed the Research and Development OU you to maintain an accurate directory structure
-Ensured the environment reflects current business operations

**Before Deletion**
![Before Deletion](Screenshots./rd-OU-before-deletion.png)

**After Deletion**
![After Deletion](Screenshots./rd-OU-after-deletion.png)

## User Account Management

### 🔐 Scenario: Delegating Password Reset Permissions
- Assigned delegated permissions to user **Philip** to reset passwords
- Used the **Delegation of Control Wizard** in Active Directory
- Selected specific task: *Reset user passwords and force password change at next logon*

#### Delegation Setup
**Delegation - Select User**
![Delegation - Select User](Screenshots./delegation-select-user-philip.png)
**Delegation - Assign Permissions**
![Delegation - Assign Permissions](Screenshots./delegation-password-reset-permissions.png)

### 🔑 Scenario: Password Reset & Enforcement
- Reset user **Sophie’s** password using delegated account (**Philip**)
- Forced password change at next login for security compliance
- Verified system prompt requiring password update

#### Password Reset Execution
**Password Reset Command**
![Password Reset Command](Screenshots./philip-password-reset-command.png)
**Force Password Change Command**
![Force Password Change Command](Screenshots./force-password-change-command.png)
**Password Change Prompt**
![Password Change Prompt](Screenshots./force-password-change-prompt.png)

### Scenario: Account Lockout
- Simulated multiple failed login attempts
- Triggered account lockout based on Group Policy settings
- Observed system lockout message during login attempt

**Account Lockout Evidence:**
![Account Lockout Error](Screenshots./account-lockout-error.png)

### 🔓 Scenario: Account Unlock
- Identified locked user account in Active Directory Users and Computers (ADUC)
- Unlocked account via user properties
- Restored access successfully

****Account Lockout Evidence**
![**Account Lockout Evidence:**](Screenshots./account-locked-properties.png)
**Account Unlocked**
![Account Unlocked](Screenshots./account-unlock-after.png)

## Group Management
### Scenario: Access to Shared Resources
- Assigned users to appropriate groups
- Demonstrated how group membership controls access

---

## Computer (Machine) Management
### 🖥️ Scenario: Viewing Domain Computers
#### Domain Computers in Active Directory
![](Screenshots./domain-computers-overview.png)

### 🏢 Scenario: Organizing Computer Objects
#### Moving Computer into Correct OU
![](Screenshots./computer-ou-organization.png)

### 🚫 Scenario: Disabling Inactive Computer Account
#### Disable Computer Account
![](Screenshots./disable-computer-account.png)

## Troubleshooting Scenarios
- User unable to log in
- Account locked out
- Access denied to shared resources

---

## Key Takeaways
- Active Directory is used to manage users, computers, and permissions
- Group-based access control simplifies permission management
- IT support relies heavily on AD for troubleshooting login and access issues

---

## Screenshots
(Add your lab screenshots here)
