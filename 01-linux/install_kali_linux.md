# How to Install Kali Linux

Kali Linux is a **Debian-based** Linux distribution designed for digital forensics and penetration testing. This note covers the basic steps to install Kali Linux on your machine, either as a **dual boot** or inside a **virtual machine**.

---

## 🛠️ Prerequisites:
- A **minimum of 20 GB** free disk space
- **4 GB of RAM** (more is better for VM installations)
- A **USB drive** (for a bootable installer)
- A **Kali Linux ISO file**: [Download here](https://www.kali.org/get-kali/)

---

## 🚀 Steps to Install Kali Linux:

### Option 1: **Installing on a Virtual Machine (VM)**
1. **Download and install VirtualBox** (or VMware).
2. Create a new VM:
   - Set the **OS type** as **Linux** and version as **Debian 64-bit**.
   - Allocate **2 GB of RAM** and **10 GB of hard disk space** (you can adjust this based on your system's specs).
3. **Attach the Kali Linux ISO** file to the VM.
4. **Boot the VM** and follow the Kali Linux installation steps:
   - Select **Graphical Install**.
   - Choose **English** and then your location.
   - Set up a **username** and **password**.
   - Choose a partitioning method (for beginners, use **Guided - use entire disk**).
5. Once installation is complete, reboot the system and **log in** with your credentials.

### Option 2: **Installing on a Physical Machine (Dual Boot)**
1. Create a **bootable USB drive** using tools like **Rufus** (for Windows) or **Etcher** (for Mac/Linux).
2. Boot your computer from the **USB drive**.
3. Select **Graphical Install** and follow the same steps as above, choosing to **install alongside** your existing operating system for dual-boot setup (not in the directory of windows)

---

## ⚙️ Post-Installation Setup:
1. **Update Kali**:
   ```bash
   sudo apt update && sudo apt upgrade
