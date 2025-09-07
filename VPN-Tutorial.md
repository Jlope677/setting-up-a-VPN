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
<img width="959" height="589" alt="whatsmyipaddress" src="https://github.com/user-attachments/assets/4c2f9c60-8d1d-47ef-bd85-72cd8bef3e0a" />


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
<img width="1125" height="681" alt="vm1" src="https://github.com/user-attachments/assets/e0154b57-0b55-4d58-ba9d-64a68bfe963b" />
<img width="1205" height="763" alt="vm2" src="https://github.com/user-attachments/assets/b589ffaa-5492-4439-a443-580e83ee870f" />
<img width="1085" height="761" alt="vm3" src="https://github.com/user-attachments/assets/8d10e1aa-f680-437d-ac95-d570a5b6e6b8" />
<img width="1199" height="840" alt="vm4" src="https://github.com/user-attachments/assets/d3597290-062e-4bc9-b2d8-a5e5867b019a" />


---

### STEP 3 – Connect to VM and Verify IP
1. Use **Remote Desktop Connection** with the VM IP and credentials.  
2. Once inside the VM, visit [www.whatismyipaddress.com].  
3. Confirm that the VM shows the external IP assigned by Azure.

**Logging into VM**  
<img width="601" height="630" alt="logging in" src="https://github.com/user-attachments/assets/bede0509-3160-4022-8a58-7c85c83ccc42" />



**VM Assigned IP (Azure – Virginia, USA)**  
<img width="1529" height="665" alt="whatsmyipaddressvm" src="https://github.com/user-attachments/assets/95d8a1db-8747-4801-bed6-f1cb39c2763d" />

---

### STEP 4 – Install and Connect Proton VPN
1. Create a **free Proton VPN account**.  
2. Log into the VM, download, and install Proton VPN for Windows.  
3. Use your Proton VPN credentials to sign in.  
4. Select a VPN server location (Japan for this demo).  

**Proton VPN Setup Screenshots**  
<img width="1446" height="708" alt="proton vpn" src="https://github.com/user-attachments/assets/83809646-c56a-41d9-8018-da7c0fff4d04" />
<img width="1587" height="897" alt="proton vpn2" src="https://github.com/user-attachments/assets/b1ba70f2-c79a-44be-b42a-d6ea4e94d82e" />
<img width="1352" height="899" alt="proton vpn3" src="https://github.com/user-attachments/assets/37223786-5f81-4391-9b8c-4834102eefc8" />
<img width="1297" height="867" alt="proton vpn4" src="https://github.com/user-attachments/assets/fac605f2-cffa-4822-9b10-0fb84a7afd2d" />


---

### STEP 5 – Verify VPN IP
1. Open [www.whatismyipaddress.com] again inside the VM.  
2. Confirm new IP address shows Japan.  

**VPN IP Address (Tokyo, Japan)**  
<img width="806" height="618" alt="myipaddressvm with vpn" src="https://github.com/user-attachments/assets/7a075fe7-afd9-4b3e-aded-54c322c479e9" />


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
