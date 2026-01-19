# Hyper-V & VMware Virtualisation

**Virtualisation** allows multiple **virtual machines (VMs)** to run on a single **physical server (host)**.

Each VM behaves like a real computer with:
- CPU
- RAM
- Disk
- Network

---
![image](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Hyper%20V%20PC%20Virtualization.png)


![image](https://github.com/Musrat-Jahan/Service-Desk-Engineer/blob/main/Images/Hyper%20v.png)

## Why companies use virtualisation

Virtualisation is used because it provides:
- Better hardware utilisation
- Lower cost (fewer physical servers)
- Faster deployment of servers
- Easier backups and recovery
- Isolation between systems
- High availability and scalability

Without virtualisation:
- One server = one workload
- More hardware cost
- Longer recovery times
- Harder scaling

---

## How virtualisation works (high level)

### Hypervisor
A **hypervisor** is the software layer that creates and manages VMs.

Two main types:
- **Type 1 (bare-metal)**: Runs directly on hardware  
  Example: Hyper-V, VMware ESXi
- **Type 2**: Runs on top of an OS (labs/testing)

Enterprise environments use **Type 1**.

---

### Host
- Physical server
- Runs the hypervisor
- Provides CPU, RAM, disk, network

---

### Virtual Machine (VM)
- Software-based computer
- Runs its own OS (Windows/Linux)
- Isolated from other VMs

---

### Management layer
- Hyper-V Manager / Failover Cluster Manager
- VMware vCenter

Used to:
- Create VMs
- Allocate resources
- Monitor health
- Perform maintenance

---

## Hyper-V vs VMware (overview)

### Hyper-V
- Built into Windows Server
- Integrated with Microsoft ecosystem
- Common in Windows-heavy environments
- Often lower licensing cost

### VMware
- Industry leader in virtualisation
- Very mature and stable
- Strong enterprise features
- Common in MSP and large environments

Both are **enterprise-grade** and widely used.

---

## Core virtualisation concepts

###  CPU virtualisation
- Physical CPU cores are shared
- VMs are allocated **vCPUs**
- Over-allocating vCPUs can cause performance issues

---

### Memory (RAM)
- RAM is allocated per VM
- Hyper-V uses **Dynamic Memory**
- VMware uses **ballooning / memory management**

Running out of RAM on a host affects **all VMs**.

---

### Storage
- Virtual disks (VHD/VHDX for Hyper-V, VMDK for VMware)
- Stored on:
  - Local disks
  - SAN
  - NAS
  - Clustered storage

Storage performance is critical.

---

### Networking
- Virtual switches
- VM NICs connect to virtual networks
- Mapped to physical NICs

Most “network issues” in VMs are misconfigured virtual switches.

---

### 5.5 Snapshots / Checkpoints
- Point-in-time VM state capture
- Useful for short-term testing
- Dangerous if left long-term

Never use snapshots as backups.

---

## Storage, networking & performance basics

### Storage considerations
- Disk latency affects all VMs
- Thin vs thick provisioning
- Snapshot growth can fill storage quickly

### Networking considerations
- VM network depends on:
  - Virtual switch config
  - Physical NICs
  - VLAN tagging

### Performance red flags
- High disk latency
- CPU ready time (VMware)
- Host memory pressure

---

##  Positive and negative sides

### ✅ Positive
- Efficient use of hardware
- Faster recovery (restore VM)
- Easy server provisioning
- Supports HA and DR
- Isolation between workloads
- Easier testing and maintenance

### ❌ Negative
- Host failure affects many VMs
- Resource contention if poorly sized
- Added complexity
- Storage mismanagement can cause outages
- Snapshots misused can cause major issues

---

##  How Service Desk engineers use virtualisation

### Typical Service Desk (L1/L2) tasks
- Start / stop VMs
- Check VM status
- Verify VM network connectivity
- Check disk space on VM
- Escalate performance issues
- Assist with restores (under guidance)
- Monitor alerts

### Common Service Desk tickets
- “The server is slow”
- “VM is offline”
- “Application server not responding”
- “Disk is full”
- “Network not reachable from VM”

Service Desk usually **does not design** virtual environments but must understand impact.

---

## Virtualisation troubleshooting mindset

### Step 1: Identify scope
- One VM?
- Multiple VMs?
- Entire host?

### Step 2: Identify layer
- Guest OS issue?
- VM resource issue?
- Host issue?
- Storage issue?
- Network issue?

### Step 3: Avoid risky actions
- Don’t reboot hosts casually
- Don’t delete snapshots blindly
- Don’t resize disks without confirmation

---

## Common issues + fixes (step-by-step)

### VM is offline

**Checks**
1. Is the host online?
2. Is the VM powered off or paused?
3. Any host alerts?

**Fix**
- Start VM
- If fails, check logs and escalate

---

###  VM is slow

**Possible causes**
- CPU contention
- Low RAM
- Disk latency
- Snapshot present

**Fix approach**
1. Check VM CPU/RAM usage
2. Check host resource usage
3. Check storage latency
4. Check for snapshots
5. Escalate if host-level issue

---

### Disk full inside VM

**Symptoms**
- Application errors
- Services fail

**Fix**
- Confirm which disk is full
- Clean up files
- Extend virtual disk (if approved)
- Expand partition inside OS

---

### Snapshot causing issues

**Symptoms**
- VM slow
- Storage filling rapidly

**Fix**
- Confirm snapshot age
- Merge/delete snapshot during maintenance window
- Monitor storage during merge

---

### VM has no network connectivity

**Checks**
1. VM NIC connected?
2. Correct virtual switch?
3. VLAN correct?
4. Guest OS IP config?

**Fix**
- Reconnect NIC
- Correct virtual switch
- Restart network adapter if needed

---

### Host storage full

**Impact**
- Multiple VMs affected
- Critical condition

**Fix**
- Identify large snapshots
- Clean unused VMs
- Expand storage (L3/infra team)
- Immediate escalation required

---

## Common tools & consoles

### Hyper-V
- Hyper-V Manager
- Failover Cluster Manager
- Event Viewer

### VMware
- vSphere Client
- vCenter
- ESXi host console

### Guest OS tools
- Task Manager / Resource Monitor
- Event Viewer
- Disk Management

---

## Safety checklist (avoid outages)

- ✅ Never treat snapshots as backups
- ✅ Don’t reboot hosts without approval
- ✅ Check impact before VM changes
- ✅ Monitor storage before deleting snapshots
- ✅ Document VM changes
- ✅ Escalate host-level issues early

---

## Interview-ready phrases

Use these confidently:

- “I determine whether the issue is at VM, host, storage, or network layer.”
- “Snapshots are short-term tools, not backups.”
- “If multiple VMs are affected, I immediately check host resources.”
- “I avoid risky actions like host reboots without change approval.”

---

## Quick cheat sheets

### VM slow checklist
- CPU over-allocated?
- RAM pressure?
- Snapshot present?
- Disk latency?
- Host overloaded?

### VM offline checklist
- Host online?
- VM state?
- Recent changes?
- Storage accessible?

### Network issue checklist
- VM NIC connected?
- Virtual switch correct?
- VLAN correct?
- Guest OS IP config?

---


