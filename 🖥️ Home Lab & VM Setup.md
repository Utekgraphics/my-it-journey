---

## 🖥️ Virtual Machine Lab Setup - Practical Experience
**Date:** Saturday, 3rd May 2026

### Overview
As part of my hands-on IT learning journey I set up 
a personal virtual machine lab on my Ubuntu host 
machine using QEMU/Virt-Manager. This was my first 
real practical experience managing multiple operating 
systems and solving real world IT problems independently.

---

### Phase 1 - First VM Installation (Windows 7)
- Installed **Windows 7** as my first ever virtual machine
- Allocated: **2G RAM** and **40G storage**
- This was purely for practice and familiarity 
  with VM setup
- Successfully booted and ran Windows 7 inside 
  Ubuntu for the first time

---

### Phase 2 - Added Kali Linux
- Installed **Kali Linux** as a second VM alongside Windows 7
- Allocated: **2G RAM** and **25G storage**
- Purpose: Learning networking, security tools 
  and cybersecurity concepts
- Kali Linux will be my primary learning environment 
  for networking and forensics

---

### Phase 3 - Removed Windows 7, Installed Windows 10
- Made a strategic decision to **delete Windows 7** 
  to free up 40G of storage
- Installed **Windows 10** as a replacement
- Allocated: **3G RAM** and **60G storage**
- Purpose: Design work (Adobe Illustrator, Photoshop) 
  and general Windows environment practice
- Successfully installed **Adobe Illustrator 2022** 
  inside Windows 10 VM ✅

---

### Phase 4 - USB Passthrough Problem & Solution
**Problem:**
USB/Flash drive was not being detected inside 
Windows 10 VM. The host machine (Ubuntu) was 
taking control of the USB device and not passing 
it through to the VM.

**What I learned:**
In QEMU/Virt-Manager USB devices don't automatically 
pass through to VMs — they have to be manually added 
through the hardware configuration.

**Solution:**
1. Added user to libvirt and kvm groups:
```bash
   sudo usermod -aG libvirt $USER
   sudo usermod -aG kvm $USER
```
2. Rebooted system to apply group changes
3. Opened Virt-Manager → Windows 10 VM → 
   View → Details
4. Clicked **Add Hardware** → USB Host Device
5. Selected the USB device from the list
6. Clicked **Finish**

**Result:** USB drive successfully detected 
inside Windows 10 VM ✅

---

### Phase 5 - Formatting the USB Drive
**Problem:**
USB drive was previously used as a bootable Ubuntu 
installer. It had a special boot partition that made 
it unrecognisable as a normal storage device.

**Solution - Reformatted via terminal:**
```bash
# Step 1 - Unmount the USB
sudo umount /dev/sda1

# Step 2 - Wipe existing boot signature
sudo wipefs -a /dev/sda

# Step 3 - Create new partition table
sudo fdisk /dev/sda
# Inside fdisk: o → n → p → 1 → Enter → Enter → w

# Step 4 - Format as FAT32
sudo mkfs.vfat -F 32 /dev/sda1

# Step 5 - Label the USB
sudo fatlabel /dev/sda1 MYUSB

# Step 6 - Verify
lsblk -f
```

**Result:** USB successfully reformatted to FAT32, 
named MYUSB, recognised by both Ubuntu and 
Windows 10 VM ✅

---

### Phase 6 - Storage Cleanup & Optimisation
Ran full system cleanup to free up disk space:
```bash
sudo apt update && sudo apt autoremove && sudo apt clean && sudo apt autoclean
sudo journalctl --vacuum-time=3d
```

**Before cleanup:**
- Used: 131G | Available: 91G | Usage: 60%

**After cleanup:**
- Used: 106G | Available: 116G | Usage: 48%

**Freed up: ~25G** ✅

---

### Current VM Lab Setup

| VM | RAM | Storage | Purpose |
|---|---|---|---|
| Windows 10 | 3G | 60G | Design work & Windows practice |
| Kali Linux | 2G | 25G | Networking & security learning |

---

### Key Lessons Learned 🤯
- Virtual machines are powerful learning tools 
  that allow you to run multiple OS environments 
  safely on one machine
- USB passthrough in QEMU requires manual 
  configuration unlike VirtualBox
- A bootable USB needs to be reformatted before 
  it can be used as normal storage again
- Regular system cleanup is important for 
  maintaining healthy disk usage
- Resource allocation (RAM and storage) requires 
  careful planning especially on limited hardware

---

### Tools Used
- **QEMU/Virt-Manager** - Virtual machine management
- **Ubuntu Terminal** - All configurations done via CLI
- **qemu-img** - VM disk management
- **fdisk & mkfs** - USB partitioning and formatting

### Status: ✅ Completed
### Next: Continuing networking studies and 
### setting up Kali Linux tools

---
