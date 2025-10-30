# Cybersecurity-home-lab
This project demonstrates how to build a personal cybersecurity lab to safely simulate attacks and defenses using virtual machines.   It serves as a foundation for future projects like vulnerability scanning, SIEM setup, and penetration testing.
 Tools & Technologies Used

| Tool | Purpose | Type |
|------|----------|------|
| **VirtualBox** | Virtualization software to create and manage multiple VMs | Virtualization |
| **VMware Workstation (Optional)** | Alternative virtualization platform | Virtualization |
| **Kali Linux** | Penetration testing and ethical hacking | OS | 
| **Windows 10** | Target system for testing vulnerabilities | OS | 
| **Ubuntu** | Defensive/server environment | OS | 

---

## ⚙️ Setup Steps

### 1. Install Virtualization Software
- Download and install **VirtualBox** (recommended) or **VMware Workstation Player**.
- Ensure **virtualization** is enabled in BIOS/UEFI.

### 2. Download OS Images
- [Kali Linux](https://www.kali.org/get-kali/)
- [Ubuntu](https://ubuntu.com/download)
- [Windows 10 ISO](https://www.microsoft.com/software-download/windows10)

### 3. Create Virtual Machines
| VM Name | OS | Role | Example IP |
|----------|----|------|-------------|
| Kali-Lab | Kali Linux | Attacker | 192.168.10.10 |
| Win10-Lab | Windows 10 | Victim | 192.168.10.11 |
| Ubuntu-Lab | Ubuntu | Server/Defender | 192.168.10.12 |

### 4. Configure Networking
- Use **Internal Network** or **Host-Only Adapter**.
- Assign manual IPs to each VM.
- Test connectivity:
  ```bash
  ping 192.168.10.11
  ping 192.168.10.12
