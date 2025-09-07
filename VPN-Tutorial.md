# VPN – Prerequisites and Installation

## Project Summary
This project demonstrates the installation and use of a VPN service (Proton VPN) in a cloud-hosted environment. The goal is to show how VPN technology can change IP addresses and mask geographic location by connecting through different endpoints.

- **Type:** Tutorial / Walkthrough  
- **Languages Used:** None (GUI and setup only)  
- **Environments Used:**  
  - Microsoft Azure Virtual Machines  
  - Windows 10 (21H2)  
  - Remote Desktop  
- **Technologies/Applications Used:**  
  - Proton VPN  
  - Internet Information Services (IIS)

---

## Media (Images)
Screenshots of each step have been included below.

---

## Demonstration

### STEP 1 – Locate Local IP
- Visit [www.whatismyipaddress.com](https://www.whatismyipaddress.com).  
- Record your home IP address.

**Original IP (Home ISP – USA, Texas)**  
![Original Home IP](whatsmyipaddress.PNG)

---

### STEP 2 – Set Up Virtual Machine in Azure
1. Navigate to [Azure Portal](https://portal.azure.com).  
2. Create a Virtual Machine:  
   - Name: **vpn-test-win-10**  
   - Region: **East US 2**  
   - Networking: Use defaults or configure as shown  
   - Size: Standard_D2s_v3 – 2 vCPUs, 8 GiB memory  
3. Select **Review + Create**, validate, then launch the VM.

**VM Setup – Example Screenshots**  
![VM Step 1](vm1.PNG)  
![VM Step 2](vm2.PNG)  
![VM Step 3](vm3.PNG)  
![VM Step 4](vm4.PNG)  

**VM Assigned IP (Azure – Virginia, USA)**  
![VM IP](whatsmyipaddressvm.PNG)

---

### STEP 3 – Connect to VM and Verify IP
1. Use **Remote Desktop Connection** with the VM IP and credentials.  
2. Once inside the VM, visit [www.whatismyipaddress.com].  
3. Confirm that the VM shows the external IP assigned by Azure.

**Logging into VM**  
![Logging In](logging in.PNG)

---

### STEP 4 – Install and Connect Proton VPN
1. Create a **free Proton VPN account**.  
2. Log into the VM, download, and install Proton VPN for Windows.  
3. Use your Proton VPN credentials to sign in.  
4. Select a VPN server location (Japan for this demo).  

**Proton VPN Setup Screenshots**  
![Proton Step 1](proton vpn.PNG)  
![Proton Step 2](proton vpn2.PNG)  
![Proton Step 3](proton vpn3.PNG)  
![Proton Step 4](proton vpn4.PNG)

---

### STEP 5 – Verify VPN IP
1. Open [www.whatismyipaddress.com] again inside the VM.  
2. Confirm new IP address shows Japan.  

**VPN IP Address (Tokyo, Japan)**  
![VPN IP](myipaddressvm with vpn.PNG)

---

## Final Results
We successfully used three different IP addresses in this lab:

- **Home IP (USA, Texas – Charter ISP)**  
- **Virtual Machine IP (Azure Datacenter – Virginia, USA)**  
- **VPN IP (Japan – Proton VPN)**  

This demonstrates how VPN services combined with cloud resources can obscure physical location and enhance privacy.

---

## Clean Up
If the VM is no longer needed, **delete it in Azure** to avoid charges.
