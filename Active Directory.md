# Active Directory (AD)

**Active Directory (AD)** is Microsoft’s directory service used to centrally manage:
- **Identities** (users, admins, service accounts)
- **Devices** (computers, servers)
- **Security** (groups, permissions)
- **Policies** (password rules, restrictions via Group Policy)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Login%20In%20Desktop.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Remote_Desktop%20Login.png)

### Objects
- **User**: a person or service identity
- **Group**: collection of users for permissions
- **Computer**: domain-joined workstation/server identity
- **OU (Organizational Unit)**: container used to organize + apply policies

### User:
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20create.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Password%20Set.png)

![images](http://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Details_Account.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Address%20details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Details%20Member%20of%20group.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Job%20details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Logon%20hours%20Details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Ad_User%20Logon%20Workstation%20details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20add%20Manager.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Properties.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Reset%20Password.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_FindSearch%20%20User1.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_%20Find%20User2.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_FindSearch%20%20User3.png)

### Groups 
- Assign permissions to **groups**
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Group%20creation1.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Group%20creation2.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Group%20details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Rename%20group.png)

- Put users into groups
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Add%20user%20in%20group.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Add%20user%20in%20group2.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Group%20details.png)

- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Remove%20user%20frome%20Group.png)
- 
- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20Details%20Member%20of%20group.png)
- Avoid giving permissions to users directly
  
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Distribution%20list_%20group%20create.png)


### Organizational Unit(OU) structure 
OUs are used to:
- Organize objects
- Target Group Policies cleanly
- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_OU%20create1.png)
- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_OU%20create2.png)
- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_OU%20option.png)


![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20create%20in%20OU.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20move%20fromOU1.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_User%20move%20fromOU2.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Create%20OU%20in%20OU1.png)

## Group Policy (GPO) basics

Group Policy is a system for enforcing settings for:
- Computers (machine settings)
- Users (user environment settings)

Examples:
- Drive mappings
- Password rules
- Windows Update settings
- Security restrictions
- Browser/desktop controls

- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/GPM%20console%20open.png)
- 
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM%20details.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM_Domains.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO_DDP%20edit.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO_DDP%20details.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM_Password%20Policy%201.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM_Password%20Policy%202.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM_Password%20Policy%203.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPM_Password%20Policy%204.png)


![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Account%20Policy1.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Ad_Account%20lockout%20policy1.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Account%20lockout%20Policy2.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Account%20lockout%20policy3.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Command%20Prompt%20open.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/CMD%20Group%20policy%20update.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20Create.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20Details.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20select.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20in%20Group.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20Linked.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20Edit.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20link%20enforced.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPO%20.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_GPME_Administrative%20Policy.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Administrative%20Policy%20_CMD1.png)
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_Administrative%20Policy%20CMD2.png)


## Why we need Active Directory

Companies use AD because it gives:
- **Central login** (one username/password for many services)
- **Central access control** (who can access what)
- **Central policy enforcement** (security settings, standards)
- **Scalability** (manage 10 users or 10,000 users)
- **Audit + compliance** (track access and changes)

Without AD, every computer and app becomes a separate island:
- More passwords
- More mistakes
- More security risk
- Harder onboarding/offboarding

---
block 
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/CMD%20Block%20Notification.png)


##  How Active Directory works 

### The “Domain” concept
A Domain is the boundary where identities and policies are managed.
Example: `company.local` or `company.com`
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Remote_Desktop%20Login.png)

![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/CMD_PC%20name.png)

###  Domain Controllers (DCs)
A Domain Controller stores the AD database and handles:
- Authenticating users and computers
- Authorizing access to resources
- Enforcing security policies

If DCs are down or broken:
- Logins fail
- Access to resources fails
- Many business services stop working
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Login%20In%20Desktop.png)
### AD database
Stored on DCs (NTDS). It contains objects like:
- Users
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/Add%20user.png)
- Groups
- 
- Computers
- OUs
- ![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Active%20Directory/AD_OU%20create1.png)
- Policies and links

### Replication
If there are multiple DCs, changes replicate between them.
Replication issues cause “it works for some users but not others”.

### DNS dependency (critical)
AD relies heavily on **DNS**.  
If DNS is wrong, AD breaks (login delays, GPO failures, domain join issues).

---

## AD authentication vs authorization

### Authentication = “Who are you?”
- Login to a domain computer
- Enter credentials
- DC verifies identity (Kerberos/NTLM)

### Authorization = “What are you allowed to access?”
- File shares
- Applications
- Printers
- Admin rights

Most tickets are one of these:
- **Can’t log in** (authentication)
- **Access denied** (authorization)

---

## Group Policy (GPO) basics

Group Policy is a system for enforcing settings for:
- Computers (machine settings)
- Users (user environment settings)

Examples:
- Drive mappings
- Password rules
- Windows Update settings
- Security restrictions
- Browser/desktop controls

### How GPO applies
Order of processing:
1. Local
2. Site
3. Domain
4. OU

### Inheritance + conflicts
- Higher-level GPOs flow down to child OUs
- You can block inheritance (dangerous if you don’t understand it)
- You can enforce a GPO (also risky)

---

## Positive and negative sides of AD

### ✅ Positive
- Central management of users, devices, and access
- Strong security control when configured properly
- Faster onboarding/offboarding
- Group-based permissions = scalable
- Consistent configuration across many devices (via GPO)
- Better auditing and compliance

### ❌ Negative
- Complex (easy to break if you don’t understand inheritance/DNS)
- Heavily dependent on DNS and time sync
- Replication can cause inconsistent behavior
- Legacy systems may rely on older protocols
- Poor design grows technical debt (messy OUs, random GPOs)

---

## How Service Desk Engineers use AD (daily tasks)

### Typical Service Desk tasks (L1/L2)
- Unlock user accounts
- Reset passwords
- Enable/disable accounts
- Create accounts (depending on company policy)
- Add/remove users from security groups
- Check group membership for access issues
- Find user/computer objects and verify status
- Identify which OU a computer/user is in
- Basic GPO checks (is policy applying?)

### Common access tickets handled using AD
- “I can’t access the shared drive”
- “My account is locked”
- “I can’t log in”
- “I need access to an app”
- “New starter setup”
- “Offboarding: disable account, remove access”

---

## AD troubleshooting mindset

### Step 1: Classify the problem
Most AD issues are:
- Authentication (login)
- Authorization (permissions)
- Group Policy
- DNS
- Replication
- Trust relationship

### Step 2: Confirm scope
- One user? Many users?
- One computer? Whole site?
- Since when? After changes?

### Step 3: Do safe checks first
- Don’t change GPOs in production blindly
- Don’t edit Default Domain Policy casually
- Prefer read-only checks → then minimal change

### Step 4: Document actions
- What you changed
- What you tested
- Outcome

---

## Common AD issues + fixes (step-by-step)

> Use these like ticket playbooks.

### Account locked out
**Symptoms**
- User gets “account locked” message

**Checks**
1. In ADUC: confirm **Locked out** status
2. Check if repeated lockouts happen (old device, cached credentials)

**Fix**
- Unlock account
- Identify source device (phone/outlook/old PC) and update saved password

**Common root causes**
- Outlook stored old password
- Mobile email profile using old password
- Mapped drive saved credentials

---

### Password reset but still can’t log in
**Possible causes**
- Logging into local account instead of domain
- Replication delay between DCs
- Cached credentials
- Wrong username format

**Fix approach**
1. Confirm login format: `DOMAIN\username`
2. Have user reboot and try again
3. If multiple DCs: check replication health (L3)

---

###  “Trust relationship failed”
**Symptoms**
- “The trust relationship between this workstation and the primary domain failed”

**Cause**
- Computer secure channel broken

**Fix**
- Remove computer from domain → reboot → rejoin domain → reboot
- Or repair secure channel (if permitted)

---

### User cannot access shared drive (Access Denied)
**What this usually means**
Authorization issue.

**Step-by-step**
1. Confirm user is in correct **security group**
2. Ask user to log off/log on (group membership updates at login)
3. Check **NTFS permissions** on folder
4. Check **Share permissions**
5. Check if drive mapping is via **GPO**
6. Confirm no GPO restriction is blocking access

**Fix**
- Add user to correct group (preferred)
- Adjust group permissions (not user permissions)
- Apply correct NTFS rights

---

### Drive mappings not showing
**Common causes**
- GPO not applying
- User/computer in wrong OU
- Security filtering incorrect
- Network connection not ready at logon

**Fix approach**
1. Confirm user OU and GPO link
2. Confirm GPO security filtering: **Read + Apply**
3. Run `gpupdate /force`
4. Check results (`gpresult`)
5. Consider enabling “Always wait for the network...” if needed (advanced)

---

### Group Policy not applying
**Common causes**
- Wrong OU
- Inheritance blocked
- WMI filter excluding device
- Permissions/security filtering wrong
- Client cannot reach DC (DNS issue)

**Fix approach**
1. Confirm OU placement
2. Confirm inheritance status
3. Confirm permissions on GPO
4. Check client DNS settings (must point to DC)
5. Force update + verify results

---

### Login is slow / “Applying Group Policy...” takes forever
**Common causes**
- DNS issues
- DC connectivity issues
- Broken scripts or drive mappings
- Too many GPOs / conflicting policies

**Fix approach**
1. Check client DNS is DC
2. Check network connectivity to DC
3. Review GPO processing with `gpresult`
4. Event Viewer → GroupPolicy logs

---

### Domain join fails
**Common causes**
- DNS not pointing to DC
- Time sync issue
- Wrong credentials / permissions
- Firewall/network blocking DC

**Fix approach**
1. Confirm client DNS points to internal DC
2. Confirm time is correct
3. Ensure domain join account has rights
4. Test connection to DC

---

### “It works for some users but not others”
This often indicates:
- Replication issues between DCs
- Different site/DC being used
- Group membership not replicated

**Fix approach (L3)**
- Check replication status and event logs

---


## Interview Questions

---

## Common Mistakes
---

## Common tools and commands

### GUI tools
- **ADUC**: Active Directory Users and Computers
- **GPMC**: Group Policy Management Console
- **Event Viewer**: Client/DC logs

### Commands (run on client)
```powershell
gpupdate /force
gpresult /r
gpresult /h C:\Temp\gp.html
ipconfig /all
whoami /groups

---

