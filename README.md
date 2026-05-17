# Windows Server 2022 VirtualBox Lab

## Objective
This lab demonstrates the installation and configuration of Windows Server 2022 using VirtualBox. The goal is to gain hands-on experience with server deployment, virtualization, and basic system administration.

---

## Tools & Requirements
- Oracle VirtualBox
- Windows Server 2022 ISO
- VirtualBox Extension Pack (recommended)

---

## Downloading Windows Server 2022

Download the official ISO from Microsoft:
<p align="center">
  <img width="1920" height="1032" alt="Screenshot 2026-05-09 201731" src="https://github.com/user-attachments/assets/9d6925e6-42a4-4572-9e78-a87b46e44d81" />
</p>
- Windows Server 2022 Evaluation ISO
- Make sure to select the x64 version

> Note: The ISO file is large and may take time to download.

---

# Creating the Virtual Machine

## Step 1: Create New VM
- Open VirtualBox
- Click **“New”**
- Name the VM: Windows Server 2022
- Select:
  - Type: Microsoft Windows
  - Version: Windows 2022 (64-bit)

---

## Step 2: Select ISO

- Choose **“Select ISO Image”**
- Load the Windows Server 2022 ISO
- Enable:
  - Skip Unattended Installation
<p align="center">
 <img width="1920" height="1080" alt="Screenshot 2026-05-09 194421" src="https://github.com/user-attachments/assets/b73b048a-002e-470c-b1b0-0be22dfb2826" />
</p>
---

## Step 3: Hardware Configuration

```text
Base Memory: 6168 MB
CPUs: 2
EFI Enabled: Yes
Disk Size: 50 GB
```

- Create virtual hard disk
- Finish setup and create VM

---

# Installing Windows Server 2022

## Installation Process
- Boot the virtual machine
- Proceed with default installation settings
- Select:
  - Windows Server 2022 Standard Evaluation (Desktop Experience)
<p align="center">
 <img width="1734" height="989" alt="Screenshot 2026-05-09 195932" src="https://github.com/user-attachments/assets/dfb7909c-3116-4ba5-bfb1-3bfc8c9b263b" />
</p>
---

## Post-Installation Setup
- Create a secure password (must be remembered)
- Complete initial configuration
<p align="center">
  <img width="1920" height="1080" alt="Screenshot 2026-05-09 200627" src="https://github.com/user-attachments/assets/0f93b18e-7cd8-4a01-b183-e405c7ea6a14" />
</p>
---

## Logging In
- Press:
```text
Ctrl + Alt + Delete
```
- Sign in using the created password
- Click "Okay" to the Networks Tab to allow your PC to be discoverable by other devices.
- And you're finished!
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-05-09 200843" src="https://github.com/user-attachments/assets/d879441b-e607-43cf-982f-9120ac9f2b57" />
<img width="1586" height="1032" alt="Screenshot 2026-05-09 202305" src="https://github.com/user-attachments/assets/43e638a5-795c-47b0-ad3f-e156c5a8cb27" />
</p>
---



# Troubleshooting Boot Issues

## Problem
Virtual machine fails to boot after creation.
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-05-16 184031" src="https://github.com/user-attachments/assets/6f4c0d51-e690-4788-8ab5-d847d582e416" />
</p>

## Solution
1. Open VirtualBox settings for the VM
2. Go to **Storage**
3. Locate controller settings
4. Replace or reselect ISO:
   - Set to Windows Server ISO (SERVER_EVALx64_en-us.iso)
5. Click OK
6. Restart the VM
<p align="center">
  <img width="1733" height="989" alt="Screenshot 2026-05-09 195606" src="https://github.com/user-attachments/assets/2c654c34-d2ae-4de0-ab18-eff966089b60" />
</p>
> After correction, the system should boot successfully.

---

# Skills Practiced
- Virtual machine creation
- Server OS installation
- BIOS/EFI configuration
- ISO management
- Boot troubleshooting
- Basic system administration

---

# What I Learned
This lab provided hands-on experience deploying Windows Server 2022 in a virtual environment, configuring system resources, and troubleshooting boot issues—core skills used in IT support and system administration roles.
