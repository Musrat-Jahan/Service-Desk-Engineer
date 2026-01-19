# Firewall, Routing & Switching — Network Fundamentals & Troubleshooting 

Networking is how devices communicate:
- Computers
- Servers
- Printers
- Phones
- Cloud services

---

### What a firewall is
A **firewall** controls traffic entering or leaving a network.

Think of it as:
- A security gate
- With rules deciding what is allowed or blocked

---

### What firewalls do
- Allow or block traffic
- Protect internal networks
- Control internet access
- Enable VPN connections

---

### Firewall rules

Each rule defines:
- Source
- Destination
- Port
- Protocol
- Action (Allow / Deny)


---

### Common firewall features
- Stateful inspection
- NAT (Network Address Translation)
- VPN (site-to-site, remote access)
- Web filtering
- Intrusion prevention (IPS)

---

### Common firewall mistakes
- Opening ports without security review
- Allowing "Any to Any"
- Forgetting rule order (top-down processing)

---
### What routing is
Routing decides:
- **Where traffic goes next**

Routers connect:
- Different networks
- Different subnets
- Different locations

---

### Default gateway
The **default gateway** is where traffic goes if it doesn’t know the destination.

If gateway is wrong:
- Internet won’t work
- External access fails

---

### Static vs dynamic routing
- **Static routing**: manually defined routes
- **Dynamic routing**: routes learned automatically (OSPF, BGP)

Service Desk mostly deals with **static routing concepts**.

---

### NAT (Network Address Translation)
- Translates private IPs to public IPs
- Allows many devices to share one public IP

If NAT breaks:
- Internet breaks

---

### What a switch does
A **switch** connects devices **inside the same network**.

Switches operate mainly at:
- Layer 2 (MAC addresses)
- Sometimes Layer 3 (advanced switches)

---

### VLANs 
VLANs logically separate networks on the same switch.

Example:
- VLAN 10: Staff
- VLAN 20: Guests
- VLAN 30: Servers

VLANs improve:
- Security
- Performance
- Network organisation

---

### Trunk vs access ports
- **Access port**: one VLAN (end devices)
- **Trunk port**: multiple VLANs (switch-to-switch, firewall)

Misconfigured VLANs cause:
- “No network” issues
- Intermittent access problems

---

## Core network concepts 

### IP Address
Unique address of a device.

Example:


If DNS fails:
- Internet looks down
- AD and M365 break

---

### DHCP
Automatically assigns IP addresses.

If DHCP fails:
- Devices get no IP
- Network access fails

---

## Why companies need firewalls, routing & switching

Companies need them for:
- Secure internet access
- Network segmentation
- Remote access (VPN)
- Site-to-site connectivity
- Cloud integration
- Performance and reliability

Without proper networking:
- Security risk
- Downtime
- Poor user experience

---

## Positives and negatives

### ✅ Positives
- Secure communication
- Controlled access
- Scalable networks
- Supports modern cloud services

### ❌ Negatives
- Misconfiguration can break everything
- Requires careful planning
- Troubleshooting can be complex
- Poor documentation causes long outages

---

## How Service Desk engineers use networking daily

### Typical Service Desk tasks
- Check IP configuration
- Verify connectivity
- Identify DNS issues
- Confirm VLAN placement
- Escalate firewall changes
- Assist with VPN issues

### Common tickets
- “No internet”
- “Can’t access server”
- “VPN not connecting”
- “Printer offline”
- “Slow network”

---

## Network troubleshooting mindset

### Golden rule
> Always start at the **lowest layer** and work up.

This is the **OSI model mindset**.

---

### Step-by-step thinking
1. Physical (cables, Wi-Fi, link lights)
2. IP address assigned?
3. Correct gateway?
4. DNS working?
5. Firewall blocking?
6. Routing correct?

Never jump straight to firewall rules.

---

## Common network issues + fixes 

### No internet access

**Checks**
1. IP address assigned?
2. Correct gateway?
3. Can ping gateway?
4. Can ping public IP (8.8.8.8)?
5. DNS resolving?

**Fix**
- DHCP issue
- DNS misconfiguration
- Firewall/NAT issue

---

### Can access internet but not internal server

**Likely causes**
- VLAN issue
- Firewall rule missing
- Routing issue

**Fix**
- Confirm VLAN
- Check firewall allow rules
- Verify route to server subnet

---

### VPN connected but no access to resources

**Common causes**
- VPN user group missing
- Firewall rules incomplete
- Split tunnelling misconfiguration

**Fix**
- Confirm group membership
- Confirm firewall policies
- Verify VPN routes

---

### Network slow

**Possible causes**
- Bandwidth saturation
- Faulty switch port
- Duplex mismatch
- DNS delays

**Fix**
- Check switch port stats
- Test multiple devices
- Escalate if core network issue

---

### Printer or device keeps dropping off network

**Common causes**
- DHCP lease changes
- Wrong VLAN
- Power-saving on switch port

**Fix**
- Assign static IP (where approved)
- Check VLAN
- Check switch logs

---

## Essential tools & commands

### Windows
```powershell
ipconfig /all
ping
tracert
nslookup
netstat



