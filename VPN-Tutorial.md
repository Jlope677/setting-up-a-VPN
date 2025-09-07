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
Throughout this walkthrough, screenshots will be added for each major step.

---

## Demonstration

### STEP 1 – Locate Local IP
- Visit [www.whatismyipaddress.com](https://www.whatismyipaddress.com).  
- Record your home IP address.

**Example 1A – Local IP Address**  
![Example 1A](images/example1a-local-ip.png)

---

### STEP 2 – Set Up Virtual Machine in Azure
1. Navigate to [Azure Portal](https://portal.azure.com).  
2. Create a Virtual Machine:  
   - Name: **VM-FranceCentral**  
   - Region: **France Central**  
   - Username/Password: Create and record credentials  
   - Networking: Configure settings to match lab requirements  
3. Select **Review + Create**, validate, then launch the VM.

**Example 2A – Azure VM Setup Page**  
![Example 2A](images/example2a-vm-setup.png)

**Example 2B – VM Region Selection (France)**  
![Example 2B](images/example2b-region.png)

**Example 2C – Username and Password Input**  
![Example 2C](images/example2c-credentials.png)

**Example 2D – Networking Tab**  
![Example 2D](images/example2d-networking.png)

**Example 2E – VM Public IP Assigned**  
![Example 2E](images/example2e-public-ip.png)

---

### STEP 3 – Connect to VM and Verify IP
1. Use **Remote Desktop Connection** and enter the VM IP + credentials.  
2. Once inside the VM, visit [www.whatismyipaddress.com].  
3. Confirm that the VM shows an IP address located in **France**.

**Example 3A – Remote Desktop Login Screen**  
![Example 3A](images/example3a-rdp-login.png)

**Example 3B – VM Login with Credentials**  
![Example 3B](images/example3b-login.png)

**Example 3C – VM IP Address Showing France**  
![Example 3C](images/example3c-france-ip.png)

---

### STEP 4 – Install and Connect Proton VPN
1. On your local computer, create a **free Proton VPN account**.  
2. Copy login URL into the VM browser.  
3. Download and install Proton VPN for Windows inside the VM.  
4. Log in with your credentials and connect to a server (e.g., **Japan**).

**Example 4A – Proton VPN Login Page**  
![Example 4A](images/example4a-proton-login.png)

**Example 4B – Proton VPN Installed and Logged In**  
![Example 4B](images/example4b-proton-installed.png)

**Example 4C – Connected to VPN in Japan**  
![Example 4C](images/example4c-vpn-japan.png)

---

### STEP 5 – Verify VPN IP
1. Open [www.whatismyipaddress.com] again from inside the VM.  
2. Confirm new IP address shows **Japan**.

**Example 4D – VPN IP Address Showing Japan**  
![Example 4D](images/example4d-japan-ip.png)

---

## Final Results
We successfully used three different IP addresses in this lab:

- **Home IP (USA):** `137.103.51.136`  
- **Virtual Machine IP (France):** `20.216.176.18`  
- **VPN IP (Japan):** `212.102.51.251`

This demonstrates how VPN services combined with cloud resources can obscure physical location and enhance privacy.

---

## Clean Up
If the VM is no longer needed, **delete it in Azure** to avoid charges.
