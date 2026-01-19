# Microsoft 365 

**Microsoft 365 (M365)** is a cloud-based productivity and identity platform that provides:
- Email
- Collaboration
- File storage
- Identity and access control
- Security and compliance tools

---

## Why companies use Microsoft 365

Companies move to Microsoft 365 because it provides:
- Cloud email (no on-prem Exchange)
- Secure remote access
- Central identity (with Entra ID)
- Built-in security features (MFA, Conditional Access)
- Scalability (add/remove users quickly)
- Reduced infrastructure cost
- Easier collaboration (Teams, SharePoint, OneDrive)

Without M365:
- Email servers need maintenance
- Remote work is harder
- Security is weaker
- Scaling is slow

---

## How Microsoft 365 works (high level)

### Tenant
A **tenant** is the company’s Microsoft 365 environment.
- Example: `company.onmicrosoft.com`
- All users, licenses, and services live inside the tenant

### Identity
Users authenticate via **Entra ID** (formerly Azure AD).

### Services
Each service (Exchange, SharePoint, Teams) is:
- Hosted by Microsoft
- Integrated with Entra ID
- Controlled via admin portals

### Licensing
Users only get services that are:
- Licensed
- Enabled

No license = no service.

---

##  Core Microsoft 365 services

###  Exchange Online (Email)

**What it is**
- Cloud-based email, calendar, and contacts

**What engineers manage**
- Mailboxes
- Mail flow
- Spam filtering
- Shared mailboxes
- Email permissions

**Common tasks**
- Create mailbox
- Fix send/receive issues
- Grant mailbox access
- Investigate spam or phishing

---

### SharePoint Online

**What it is**
- Cloud document management and intranet platform

**What engineers manage**
- Sites
- Permissions
- Storage
- Sharing policies

**Important concept**
- SharePoint permissions ≠ NTFS permissions
- Permissions are role-based (Owner, Member, Visitor)

---

###  OneDrive for Business

**What it is**
- Personal cloud storage for each user

**Key facts**
- Tied to user account
- Deleted when user is deleted (unless retained)

**Common tasks**
- Restore deleted files
- Transfer data during offboarding

---

### Microsoft Teams

**What it is**
- Chat, meetings, calling, and collaboration

**What engineers manage**
- Teams creation
- Guest access
- Meeting issues
- Calling problems

**Dependencies**
- Teams depends on Exchange + SharePoint + OneDrive

---

## Identity: Entra ID (Azure AD)

### What it is
Cloud-based identity and access management system.

### Key concepts
- Users
- Groups
- Roles
- MFA
- Conditional Access

### Entra ID vs On-Prem AD
| Feature | Entra ID | On-Prem AD |
|------|--------|-----------|
| Cloud-native | Yes | No |
| Kerberos | No | Yes |
| Group Policy | No | Yes |
| MFA | Built-in | External |
| Device trust | Yes | Yes |

---

## Licensing basics

### Why licensing matters
Most M365 issues come down to **missing or incorrect licenses**.

### Common license types
- Business Basic
- Business Standard
- Business Premium
- E3 / E5

### Troubleshooting rule
> If something doesn’t work, **check the license first**.

---

## Security fundamentals (what engineers must know)

### Multi-Factor Authentication (MFA)
- Prevents account compromise
- Mandatory in modern environments

### Conditional Access
Rules like:
- Require MFA outside office
- Block logins from risky countries
- Require compliant device

###  Email security
- Anti-spam
- Anti-phishing
- Safe links
- Safe attachments

---

## How Service Desk engineers use Microsoft 365

### Daily Service Desk tasks
- Create users
- Assign licenses
- Reset passwords
- Enable/disable MFA
- Fix email issues
- Grant mailbox access
- Restore OneDrive files
- Add users to Teams or SharePoint
- Investigate phishing emails

### Common tickets
- “I can’t log in”
- “My email stopped working”
- “Teams won’t load”
- “I can’t access a SharePoint site”
- “I deleted a file by mistake”
- “New starter setup”
- “Offboarding user”

---

## Microsoft 365 troubleshooting mindset

### Step 1: Identify the service
Is it:
- Login (identity)
- Email
- Teams
- SharePoint
- OneDrive

### Step 2: Check licensing
No license = no access.

### Step 3: Check account status
- Enabled?
- Sign-in blocked?
- MFA issues?

### Step 4: Check service health
Microsoft outages happen.

### Step 5: Check permissions
Group membership matters.

---

## 10. Common issues + fixes (step-by-step)

### User cannot log in

**Possible causes**
- MFA problem
- Sign-in blocked
- Password expired
- Conditional Access policy

**Fix**
1. Check user sign-in status
2. Reset MFA if needed
3. Review Conditional Access
4. Reset password (if required)

---

### Email not sending or receiving

**Common causes**
- No Exchange license
- Mailbox over quota
- Outlook profile corrupted
- Spam filtering

**Fix**
1. Check license
2. Check mailbox status
3. Check mail flow
4. Recreate Outlook profile

---

### Teams not working

**Common causes**
- Missing Teams license
- Exchange Online disabled
- Cache issues
- Microsoft outage

**Fix**
1. Check license
2. Confirm mailbox exists
3. Clear Teams cache
4. Check service health

---

###  Cannot access SharePoint site

**Common causes**
- Permission not granted
- Access via wrong account
- Sharing disabled

**Fix**
1. Confirm site permissions
2. Add user to correct group
3. Verify external sharing settings

---

### MFA not working / user locked out

**Fix**
1. Reset MFA methods
2. Re-register authentication
3. Verify Conditional Access policy

---

###  Deleted user / mailbox recovery

**Important**
- Deleted users can be recovered within **30 days**

**Fix**
- Restore user
- Reassign license
- Verify mailbox and OneDrive

---

## Admin portals you must know

- Microsoft 365 Admin Center
- Entra ID Admin Center
- Exchange Admin Center
- SharePoint Admin Center
- Teams Admin Center
- Security & Compliance Center

Knowing where to look saves time.

---

## Safety checklist (avoid outages)

- ✅ Check license before troubleshooting
- ✅ Don’t disable MFA casually
- ✅ Test Conditional Access carefully
- ✅ Be careful with global admin roles
- ✅ Follow least privilege
- ✅ Document changes
- ✅ Confirm before deleting users

---

## Interview-ready phrases

Use these confidently:

- “I always check licensing first when troubleshooting M365.”
- “Most login issues are MFA or Conditional Access related.”
- “Teams relies on Exchange and SharePoint, so I check dependencies.”
- “I verify permissions rather than assigning access directly.”

---

##  Quick cheat sheets

### Login issue checklist
- Account enabled?
- License assigned?
- MFA registered?
- Conditional Access blocking?
- Service health OK?

### Email issue checklist
- Exchange license?
- Mailbox exists?
- Quota exceeded?
- Spam filtering?
- Outlook profile healthy?

### Teams issue checklist
- Teams license?
- Exchange Online enabled?
- Cache cleared?
- Microsoft outage?

---

