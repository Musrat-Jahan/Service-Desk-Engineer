
# Ticketing System 

A **ticketing system** is a central platform used to:
- Track IT issues and requests
- Assign work to engineers
- Record actions taken
- Measure response and resolution times
- Meet SLAs and compliance requirements

---
![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/new%20customer%20create.png)


![images](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/ticket%20create.png)

***Ticket Status**

Ticket status shows the current stage of a ticket in its lifecycle. Using the correct status helps with tracking, reporting, and communication.

*Open → In Progress → (Escalated / Scheduled / Onsite Job / Waiting for Vendor / Contact User) → Resolved → Closed*

**Open**: Ticket has been created and acknowledged but work has not started yet.

Used:
-New ticket logged
-Awaiting assignment or triage

**In Progress**: Work has started and the issue is actively being investigated or fixed.

Used:
-Engineer is troubleshooting
-Changes or fixes are being applied

**Escalated**: Ticket has been passed to a higher support level or specialist team.

Used:
-Issue cannot be resolved at current level
-Requires System Admin, Network & Security, or vendor support

**Scheduled**: Work is planned for a future date or maintenance window.

Used:
-Onsite visit booked
-Upgrade or installation planned
-Change requires approval or downtime window

**Onsite Job**:
-Engineer is physically attending the client or site.

Used:
-Hardware replacement
-Network cabling or device setup
-Issue cannot be resolved remotely

**Waiting for Vendor**: Resolution depends on a third-party vendor or supplier.

Used:
-Hardware under warranty
-Software vendor investigation
-ISP or cloud provider issue

**Contact User / Client**: Waiting for response, confirmation, or action from the user or client.

Used:
-Need more information
-User testing required
-Approval or confirmation pending

**Resolved** : Issue has been fixed and service is restored.

Used :
-Solution applied
-Awaiting user confirmation before closure

**Closed**: Ticket is fully completed and formally closed.

Used :
-User confirms resolution
-No response after agreed follow-up period
-Ticket completed and documented


---
**Ticket Groups / Departments**

Ticket groups define who owns the ticket and who is responsible for resolution. Correct grouping ensures faster handling, proper escalation, and clear accountability.
***Helpdesk*** 

Role: First point of contact (Level 1 support)

Responsibilities:

Log and categorise tickets
Initial troubleshooting and quick fixes
User communication and updates
Password resets and basic access issues
Escalate when required

Typical Tickets:

Basic software issues
Login or password problems
Printer and peripheral issues
How-to and general requests

Escalation:
→ System Admin / Network & Security / ICT Dept

***ICT Department*** 

Role: Overall IT operations and coordination

Responsibilities:

Own IT service delivery
Coordinate between technical teams
Handle cross-system issues
Approve upgrades, changes, and major requests
Vendor coordination and asset management

Typical Tickets:

Major incidents affecting multiple teams
IT service requests and approvals
Hardware procurement and lifecycle management
Organisation-wide upgrades or rollouts


***System Administrator***

Role: Level 2 / Level 3 infrastructure support

Responsibilities:

Server and system administration
User accounts, permissions, and policies
Backup, recovery, and system monitoring
Patch management and system upgrades

Typical Tickets:

Server failure or alerts
Active Directory and Group Policy issues
Microsoft 365 tenant administration
Storage and backup problems

***Network & Security***

Role: Network reliability and security enforcement

Responsibilities:
Network performance and availability
Firewall and security rule management
VPN and remote access support
Security incident response
Identity protection and MFA enforcement

Typical Tickets:

Internet or network outages
VPN connection issues
Firewall rule requests
Security alerts or suspicious activity

***HR Department***

Role: People-related access and compliance

Responsibilities:
Employee onboarding and offboarding requests
Role-based access approval
HR system access management
Compliance and policy alignment

Typical Tickets:
New starter account creation
Access removal for leavers
HR system login issues
Employment or policy-related access requests

Note:
HR usually approves access, while ICT teams implement it.

Typical Ticket Flow

Ticket logged → Helpdesk
Resolved at L1 or escalated
Routed to System Admin / Network & Security / ICT Dept
HR approval if people or role based


**ticketing type** 
1. Incident: Something is broken or not working. Needs quick fix to restore service.
Goal: Restore normal service ASAP
Example:

Internet not working

Cannot log in to email

Server is down

Printer not responding


2. Service Request : User is asking for something, not reporting a problem. Planned and routine work.
Goal: Provide a service
Example:

Request for new laptop

Software installation

Access to shared folder

Password reset


3. Problem :The root cause of one or more incidents. Used when incidents keep happening.
Goal: Find and remove the root cause
Example:

Wi-Fi disconnects every day

Same server crashes repeatedly

Repeated login failures due to system bug


4. Change Request : Request to change something in the system. Needs approval and planning.
Implement change safely with minimal risk
Example:

Firewall rule change

Server upgrade

Network configuration change

Software version upgrade


***Ticket Item***
 **Error**

Something goes wrong, usually with a clear message (e.g., “Outlook error 0x…”). May be one user or many.

### **Bug**

A software defect. Reproducible steps usually exist. Often needs dev/vendor.

### **Failure**

A component stopped working (disk failed, switch died, service won’t start). More “broken” than “error”.

### **Outage**

Service is down/unavailable for multiple users or a whole site (internet down, email down). Usually **P1/P2**.

### **General Request**

User asks for something new or help that isn’t “broken” (access request, how-to, new mailbox, new user setup).

### **Upgrade**

Move to a newer version / patch / feature release (Windows update plan, firmware upgrade, M365 plan change).

### **Installation**

Install software/hardware (new printer setup, install Teams, deploy agent, laptop build).

### **Performance**

Slow system/service (Wi-Fi slow, PC lagging, app takes 2 minutes to load). Needs measurements and pattern.



 Example 

* **Outage:** “Wi-Fi down at Darwin site – multiple users unable to connect”
* **Failure:** “Core switch PSU failure – intermittent network dropouts”
* **Bug:** “App crashes when exporting PDF (steps to reproduce included)”
* **Error:** “Outlook sign-in error 0x… for user”
* **General request:** “Request: access to shared mailbox Finance”
* **Installation:** “Install Adobe Reader on laptop CDU-123”
* **Upgrade:** “Upgrade Windows 11 23H2 rollout for 10 devices”
* **Performance:** “VPN slow after 5pm – high latency reported”

---

## “Priority rule”

* **P1 (Critical):** Outage + many users + no workaround
* **P2 (High):** Major function impacted / several users / limited workaround
* **P3 (Medium):** Single user or minor function impacted / workaround exists
* **P4 (Low):** Cosmetic issue, info request, scheduled install/upgrade

---
### Ticket Categories
***Business Hardware***

Used for: End-user devices and office equipment.

Subcategories

Laptop / Desktop

Monitor / Dock / Keyboard / Mouse

Printer / Scanner

Mobile Phone / Tablet

Accessories & Peripherals

Common Tickets

Device not turning on

Broken screen or battery issue

Printer not printing

New laptop setup

***Production Hardware***

Used for: Core infrastructure and critical equipment.

Subcategories

Servers (Physical)

Storage (NAS / SAN)

Backup Devices

Racks / Power / UPS

On-prem Data Centre Equipment

Common Tickets

Server hardware failure

Disk or RAID failure

UPS alert or power issue

Hardware replacement planning

***Software***

Used for: Operating systems and non-business-specific software.

Subcategories

Operating System (Windows / macOS / Linux)

Office Applications (Microsoft 365 apps)

Utilities & Tools

Drivers & Updates

Antivirus / Endpoint Agent

Common Tickets

Application crash

Software installation

Update failure

License activation issue

***Network & Security***

Used for: Connectivity, access, and protection.

Subcategories

LAN / WAN / Wi-Fi

VPN / Remote Access

Firewall / Routing / Switching

Active Directory / Identity

MFA / Password / Access Control

Security Incident / Alert

Common Tickets

Internet outage

VPN connection failure

Account locked out

Firewall rule request

***General***

Used for: Non-technical or mixed requests.

Subcategories

How-to / Guidance

Access Request (Non-system)

Information Request

Policy or Process Question

Other / Unclear

Common Tickets

How to use Microsoft Teams features

IT policy clarification

New starter checklist query

***Business Application***

Used for: Organisation-specific or third-party business systems.

Subcategories

ERP / Accounting (Xero, MYOB, SAP)

CRM Systems

HR / Payroll Systems

Industry-specific Applications

Reporting & Dashboards

Common Tickets

Application error or bug

Access or role change

Data sync issue

Performance problem

---
🧑‍💻 Ticket Groups / Departments

Ticket groups define who owns the ticket and who is responsible for resolution. Correct grouping ensures faster handling, proper escalation, and clear accountability.

1️⃣ Helpdesk

Role: First point of contact (Level 1 support)

Responsibilities:

Log and categorise tickets

Initial troubleshooting and quick fixes

User communication and updates

Password resets and basic access issues

Escalate when required

Typical Tickets:

Basic software issues

Login or password problems

Printer and peripheral issues

How-to and general requests

Escalation:
→ System Admin / Network & Security / ICT Dept

2️⃣ ICT Department

Role: Overall IT operations and coordination

Responsibilities:

Own IT service delivery

Coordinate between technical teams

Handle cross-system issues

Approve upgrades, changes, and major requests

Vendor coordination and asset management

Typical Tickets:

Major incidents affecting multiple teams

IT service requests and approvals

Hardware procurement and lifecycle management

Organisation-wide upgrades or rollouts

3️⃣ System Administrator

Role: Level 2 / Level 3 infrastructure support

Responsibilities:

Server and system administration

User accounts, permissions, and policies

Backup, recovery, and system monitoring

Patch management and system upgrades

Typical Tickets:

Server failure or alerts

Active Directory and Group Policy issues

Microsoft 365 tenant administration

Storage and backup problems

4️⃣ Network & Security

Role: Network reliability and security enforcement

Responsibilities:

Network performance and availability

Firewall and security rule management

VPN and remote access support

Security incident response

Identity protection and MFA enforcement

Typical Tickets:

Internet or network outages

VPN connection issues

Firewall rule requests

Security alerts or suspicious activity

5️⃣ HR Department

Role: People-related access and compliance

Responsibilities:

Employee onboarding and offboarding requests

Role-based access approval

HR system access management

Compliance and policy alignment

Typical Tickets:

New starter account creation

Access removal for leavers

HR system login issues

Employment or policy-related access requests

Note:
HR usually approves access, while ICT teams implement it.

---
Ticketing systems provide:
- Accountability
- Clear ownership
- Historical records
- SLA tracking
- Reporting and audits
- Consistent service delivery

Without tickets:
- Issues get forgotten
- No proof of work
- Poor communication
- SLA breaches
- Customer dissatisfaction

---

## How a ticketing system works 

### Typical ticket lifecycle

1. **Ticket created**
   - User submits via email, portal, or phone
2. **Categorised**
   - Incident / Request / Change
3. **Prioritised**
   - Based on impact and urgency
4. **Assigned**
   - To L1, L2, or L3
5. **Worked**
   - Troubleshooting, communication, fixes
6. **Resolved**
   - Solution implemented
7. **Closed**
   - User confirmation or auto-close

Every step must be documented.

---

## Common ticket types

### Incident
Something is broken.
- “I can’t log in”
- “Email not working”
- “Server is down”

### Service Request
User wants something.
- New account
- Access to folder
- Software install

### Change Request
Planned modification.
- Firewall rule change
- Server upgrade
- GPO change

Change requests usually require approval.

---

## Ticket priority vs severity 

Many people confuse these.

### Severity (Impact)
How bad the issue is technically.
- Server down = high severity
- One user issue = low severity

### Priority (Business urgency)
How urgently it must be fixed.
- CEO can’t email = high priority
- Test user issue = low priority

Priority = **Impact + Urgency**

---

## SLAs

**SLA (Service Level Agreement)** defines:
- Response time
- Resolution time

### Example SLA
| Priority | Response | Resolution |
|-------|---------|-----------|
| P1 | 15 mins | 4 hours |
| P2 | 1 hour | 8 hours |
| P3 | 4 hours | 3 days |

Breaking SLAs damages trust and contracts.

---

## How Service Desk engineers use tickets 

### Typical L1 responsibilities
- Answer calls / emails
- Create accurate tickets
- Gather information
- Fix basic issues
- Escalate when needed

### L1 ticket focus
- Password resets
- Account unlocks
- Basic M365 issues
- Printer problems
- First response communication

L1 should **never guess**. If unsure, escalate.

---

## How Level 2 engineers handle tickets

### L2 responsibilities
- Handle escalated tickets
- Troubleshoot deeper issues
- Work on servers, AD, M365
- Identify root cause
- Update ticket clearly

### L2 mindset
- Fix the problem
- Prevent recurrence
- Document for L1

---

## How Level 3 engineers handle tickets

### L3 responsibilities
- Complex infrastructure issues
- Design-level decisions
- Major outages
- Security incidents
- Root cause analysis
- Long-term fixes

### L3 tickets often involve
- Multiple systems
- Change management
- Vendor escalation

---

## Ticket notes

### Good ticket notes include
- What the issue was
- What you checked
- What you changed
- Result of the change
- Next steps

### Example (good)
