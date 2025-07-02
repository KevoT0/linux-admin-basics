# 🐧 Linux Fundamentals (Module 3)

## 📘 Overview

This hands-on module provides foundational experience with the Linux operating system through command-line interface (CLI) tasks. It focuses on system navigation, file management, user and group administration, permission handling, network diagnostics, and basic package management — all essential skills for aspiring sysadmins and IT professionals working in hybrid environments.

---

## 🧰 Tools & Technologies

- **OS Environment**: Ubuntu Desktop (via VirtualBox)
- **Utilities**: Bash Terminal, APT Package Manager
- **Platform**: Oracle VirtualBox (local virtualization)

---

## 🚦 Learning Objectives

By completing this module, you will be able to:

- Navigate the Linux file system and manage files/folders via CLI
- Create and manage users, groups, and permissions
- Modify access rights using `chmod`, `chown`, and `usermod`
- Use `ip`, `ping`, and `apt` to verify connectivity and install/remove packages
- Understand Linux directory structures and administrative boundaries

---

## 🧪 Lab Walkthrough

### 🔹 Part 1: File System Navigation & Management

**Commands Used**: `mkdir`, `cd`, `pwd`, `ls`, `touch`, `cp`, `mv`, `rm`

- Created nested directories (`my_documents`, `projects/web_dev`)
- Navigated the file system using basic CLI navigation tools
- Created, listed, copied, renamed, and deleted files and folders

<p align="center">
<img src="https://imgur.com/K5L57JO" height="80%" width="80%" alt="Linux Directory Navigation and Creation"/>
</p>

---

### 🔹 Part 2: User Management & Permissions

**User Creation**:  
Created `linuxuser1` and attempted privileged operations to confirm non-admin status.

<p align="center">
<img src="https://i.imgur.com/37.png" height="80%" width="80%" alt="Linux User Creation"/>
<br />
<img src="https://i.imgur.com/38.png" height="80%" width="80%" alt="Linux Login Screen"/>
<br />
<img src="https://i.imgur.com/39.png" height="80%" width="80%" alt="Linux Standard User Sudo Test"/>
</p>

**Sudo Privileges**:  
Added `linuxuser1` to the `sudo` group using `usermod` and verified sudo capabilities.

<p align="center">
<img src="https://i.imgur.com/40.png" height="80%" width="80%" alt="Linux Add User to Sudo Group"/>
</p>

**Shared Directory Permissions**:  
Created `/shared_linux_data`, set ownership to `root:sharedgroup`, and permissions to `770`.

<p align="center">
<img src="https://i.imgur.com/41.png" height="80%" width="80%" alt="Linux Chmod 770"/>
<br />
<img src="https://i.imgur.com/42.png" height="80%" width="80%" alt="Linux Chown Shared Group"/>
</p>

**Permission Testing**:  
Verified that `linuxuser1` could write to `/shared_linux_data` but not access `/root`.

<p align="center">
<img src="https://i.imgur.com/43.png" height="80%" width="80%" alt="Linux Permission Testing"/>
</p>

**User & Group Cleanup**:  
Successfully removed `linuxuser1` and `sharedgroup`.

<p align="center">
<img src="https://i.imgur.com/44.png" height="80%" width="80%" alt="Linux User and Group Deletion"/>
</p>

---

### 🔹 Part 3: Networking & Package Management

**Network Configuration & Testing**:

- Verified IP address using `ip a`
- Confirmed internet connectivity using `ping google.com`

<p align="center">
<img src="https://i.imgur.com/45.png" height="80%" width="80%" alt="Linux IP Address and Ifconfig Install"/>
</p>

**APT Package Management**:

- `apt update` to refresh package lists  
- `apt upgrade` to update installed software  
- Installed and removed `htop` as an example utility

<p align="center">
<img src="https://i.imgur.com/46.png" height="80%" width="80%" alt="Linux Apt Install Net-Tools and Ifconfig"/>
<br />
<img src="https://i.imgur.com/47.png" height="80%" width="80%" alt="Linux Ping Google and Apt Update"/>
<br />
<img src="https://i.com/48.png" height="80%" width="80%" alt="Linux Apt Install Htop"/>
<br />
<img src="https://i.imgur.com/49.jpg" height="80%" width="80%" alt="Htop Running"/>
<br />
<img src="https://i.imgur.com/50.png" height="80%" width="80%" alt="Linux Apt Remove Htop"/>
</p>

---

## 🧠 Skills Demonstrated

### 💻 Operating System Administration
- Ubuntu Desktop (CLI-focused)
- User and group lifecycle management
- File ownership and permissions (`chmod`, `chown`, `usermod`)
- Safe deletion and directory management

### 🌐 Networking & Connectivity
- IP address inspection via `ip a`
- Basic internet troubleshooting via `ping`
- Understanding how interfaces behave in virtualized environments

### 📦 Software & Package Management
- APT: `update`, `upgrade`, `install`, `remove`
- Monitoring and verifying running processes (`htop`)

### 🔒 Security & Access Control
- Principle of least privilege (standard vs sudo user)
- Group-based access to shared resources
- Restricted directory access testing (`/root`)

### 🧾 Command-Line Proficiency
- **Linux**: `pwd`, `ls`, `cd`, `mkdir`, `rm`, `touch`, `cp`, `mv`, `whoami`, `id`, `sudo`, `adduser`, `deluser`, `usermod`, `addgroup`, `delgroup`, `apt`
- **Networking**: `ip`, `ping`

### ☁️ Virtualization
- VirtualBox configuration for Ubuntu Desktop
- Understanding NAT and how Linux VMs access host networks

---
