# 🎫 osTicket Lifecycle Management Lab

## 📌 Project Summary
This tutorial outlines the lifecycle of a ticket from **intake to resolution** within the open-source help desk ticketing system **osTicket**. The project demonstrates my ability to configure, manage, and document the ticket lifecycle in a professional IT environment.

### Environments and Technologies Used
- **Microsoft Azure** (Virtual Machines / Compute)
- **Remote Desktop**
- **Internet Information Services (IIS)**
- **osTicket (Open-Source Ticketing System)**

### Operating Systems Used
- **Windows 10 (21H2)**

### Ticket Lifecycle Stages
1. **Intake** – End-user submits a ticket describing an issue or request.  
2. **Assignment & Communication** – Ticket is triaged, assigned to the correct department/team, and user communication begins.  
3. **Working the Issue** – Assigned agent investigates, escalates if necessary, and documents troubleshooting steps.  
4. **Resolution** – The issue is resolved, verified, and ticket is closed with proper documentation.




## 📝 Lab Setup
- **Admin/Analyst Login Page:** [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)  
- **End Users osTicket URL:** [http://localhost/osTicket](http://localhost/osTicket)  

### Initial Configuration
- Changed the **SysAdmins Department** to a **Top Level Department** to give it broader permissions and higher authority for escalations.  
- Deleted the **Maintenance Department** because before deletion, all tickets were being misrouted there by default, causing confusion and delays.  

**SysAdmins Department**  
<img width="1240" height="297" alt="Change the SysAdmins Department to a Top Level Department(1)" src="https://github.com/user-attachments/assets/828b0b51-c1b8-4ce3-b075-f576734636ac" />  
<img width="1023" height="886" alt="Change the SysAdmins Department to a Top Level Department(2)" src="https://github.com/user-attachments/assets/5dcae3b6-ecbf-45ac-a395-9020b2dae3a0" />  

**Maintenance Department**  
<img width="1336" height="565" alt="DELETE the Maintenance Department" src="https://github.com/user-attachments/assets/6ce4d2e5-c7b3-41a2-a25c-768dce57ff9c" />  

**Reflection:** Setting up departments properly makes a big difference. By deleting Maintenance, tickets could flow where they belonged, and by elevating SysAdmins to a top-level department, I ensured critical issues could be escalated with the right level of access and visibility.

---

## 🖼️ Media
Throughout this lab I included screenshots to demonstrate each step, from system setup to ticket creation, updates, and resolution. These images verify the successful implementation of osTicket as a functioning ticketing system.

---

## 🎥 Demonstration

The following tickets illustrate the end-to-end functionality of the system:

### 🎟️ Ticket 1: Online Banking Outage
**Scenario:** End user reports the entire mobile/online banking system is down.  

(original Ticket 1 content preserved below)

 Online Banking Outage
**Scenario:** End user reports the entire mobile/online banking system is down.

### Ticket Creation
- User: *Karen Doe* (Email: karen@lognpacific.com)
- Help Topic: **Report a Problem**
- Summary: *entire mobile/online banking system is down*
- Description: *Employees unable to access online banking; occasional logins fail.*

<img width="1000" height="569" alt="create ticket" src="https://github.com/user-attachments/assets/ca5a8528-36b3-484d-91bf-f0de5ad01b53" />
<img width="866" height="885" alt="create ticket2" src="https://github.com/user-attachments/assets/be42140c-85aa-4eb3-9e27-0624f8808419" />
<img width="849" height="391" alt="create ticket3" src="https://github.com/user-attachments/assets/bc1f1384-ba2d-4678-a134-425c8eaecc9c" />




### John’s Updates
- Updated SLA from *Default* → **Sev-A (Critical, 1 hour, 24/7)**.
- Changed Help Topic to **Business Critical Outage**.
- Assigned ticket to **Online Banking Team** with notes.

<img width="676" height="498" alt="john1" src="https://github.com/user-attachments/assets/8fd8478a-1a1e-479a-951c-03c1a7846344" />
<img width="1391" height="455" alt="john2" src="https://github.com/user-attachments/assets/472802bc-a9dc-4586-8b65-eb88e7aa5321" />
<img width="1350" height="618" alt="john3" src="https://github.com/user-attachments/assets/5a520395-3fea-4da7-a8cd-f0083cd3c6e2" />
<img width="1325" height="698" alt="john4" src="https://github.com/user-attachments/assets/7ea019e0-639f-41bf-bbfd-873de0284a2c" />
<img width="1314" height="681" alt="john5" src="https://github.com/user-attachments/assets/372954e7-6c4a-4a7e-ae3a-003a1807fed2" />
<img width="1321" height="689" alt="john6" src="https://github.com/user-attachments/assets/57108080-6f82-4f39-ac7d-5ef33c30f1ee" />







### Jane’s Resolution
- Reassigned the ticket to herself.
- Replied to the end user with initial troubleshooting steps.
- Confirmed root cause (bad update), rolled it back, and notified vendor.
- Marked the ticket **Resolved**.

<img width="700" height="578" alt="jane" src="https://github.com/user-attachments/assets/4316a78f-1971-4e0d-88fe-43767d02de9e" />
<img width="1376" height="640" alt="jane1" src="https://github.com/user-attachments/assets/31383464-949f-4a0d-bbec-81526a970fc1" />
<img width="1448" height="933" alt="jane2" src="https://github.com/user-attachments/assets/15a9ba19-2790-40d0-9c89-1cf6133996af" />
<img width="1321" height="850" alt="jane3" src="https://github.com/user-attachments/assets/c9b2569d-3209-41f2-9973-67807473b80e" />
<img width="1343" height="880" alt="jane4" src="https://github.com/user-attachments/assets/a48f65d7-208f-4a8e-9989-505e67db974e" />
<img width="1424" height="541" alt="jane5" src="https://github.com/user-attachments/assets/e1f0fff8-2945-4557-b3a7-3c29a63b87e2" />







**Reflection:** This ticket showed the full lifecycle—intake, escalation, reassignment, communication, and resolution. The hand-off between John and Jane mirrors real-world teamwork in critical incidents.

---



---

### 🎟️ Ticket 2: Adobe Upgrade Request
**Scenario:** Accounting department requests an Adobe software upgrade.  

(original Ticket 2 content preserved below)

 Adobe Upgrade Request
**Scenario:** Accounting department requests an Adobe software upgrade.

### Ticket Creation
- User: *Ken Doe* (Email: ken@lognpacific.com)
- Help Topic: **General Inquiry / Other**
- Summary: *Accounting department needs Adobe upgrade*
- Description: *Many users can’t use Adobe software.*

<img width="972" height="921" alt="ticket2(1)" src="https://github.com/user-attachments/assets/01eb5d80-9ad2-4ea9-971e-87e24737f3ee" />
<img width="979" height="551" alt="ticket2(2)" src="https://github.com/user-attachments/assets/510b667f-267a-4b57-9186-f8fbbe22f829" />




### John’s Updates
- Changed SLA from *Default* → **Sev-C**, with justification: only 2 users impacted.
- Assigned the ticket to himself.
<img width="1132" height="482" alt="johnb(1)" src="https://github.com/user-attachments/assets/bb32bdef-957f-440d-a1ad-bf9a8e444934" />
<img width="1082" height="730" alt="johnB(2)" src="https://github.com/user-attachments/assets/7b9f05c2-abdf-4cbe-b657-28db919e0e64" />
<img width="1109" height="711" alt="johnB(3)" src="https://github.com/user-attachments/assets/7c6317a9-873d-447b-a9fb-f3d70be871cb" />
<img width="1099" height="565" alt="johnB(4)" src="https://github.com/user-attachments/assets/b50ecdf7-15e6-41ef-8749-8ef285b914c0" />





### Resolution
- Documented troubleshooting via internal notes.
- Restart fixed the issue.
- Ticket marked **Resolved**.

<img width="1098" height="847" alt="johnB(5)" src="https://github.com/user-attachments/assets/5099474d-0579-4065-ae73-8cf7cc292fbc" />
<img width="1118" height="796" alt="johnB(6)" src="https://github.com/user-attachments/assets/633c0177-2dce-440e-8a7e-08f61a15004f" />
<img width="1093" height="696" alt="johnB(7)" src="https://github.com/user-attachments/assets/b24048ed-c45f-4b3f-a004-4ebe7dfd5a19" />
<img width="1131" height="496" alt="johnB(8)" src="https://github.com/user-attachments/assets/8b8d27f2-258f-4d69-812f-0da56ec8fe4a" />


⚠️ **Note on Permissions:** John should have had reply permissions, but I overlooked it. Because of this, he only used internal notes. In a real-world setting, I would have corrected the agent role permissions so he could communicate directly with the user.

**Reflection:** Even smaller tickets require proper classification and documentation. I learned that making sure roles are set up correctly is critical for smooth communication.

---



---

### 🎟️ Ticket 3: CFO’s Laptop Will Not Turn On
**Scenario:** End user reports the CFO’s laptop won’t power on.  

(original Ticket 3 content preserved below)

 CFO’s Laptop Will Not Turn On
**Scenario:** End user reports the CFO’s laptop won’t power on.

### Ticket Creation
- User: *Karen Doe* (Email: karen@lognpacific.com)
- Help Topic: **Personal Computer Issues**
- Summary: *CFO’s laptop will no longer turn on*
- Description: *Laptop won’t turn on despite pressing the power button.*

<img width="815" height="935" alt="ticket3(1)" src="https://github.com/user-attachments/assets/290a3fc1-14de-4f73-8986-ade60ab212d1" />
<img width="811" height="461" alt="ticket3(2)" src="https://github.com/user-attachments/assets/242779f8-0a76-4be4-82ea-303b5db1b7ef" />



### John’s Updates
- Updated priority from *Normal* → **Emergency**.
- Changed SLA from *Default* → **Sev-B**, with note that it may be reclassified.
- Assigned ticket to himself.

<img width="959" height="449" alt="johnC(1)" src="https://github.com/user-attachments/assets/a977eb5d-a502-4394-8633-1d60ea9073e5" />
<img width="911" height="410" alt="johnC(2)" src="https://github.com/user-attachments/assets/0d5c96f9-fc25-457d-9d92-1c3c43680b20" />
<img width="959" height="565" alt="johnC(3)" src="https://github.com/user-attachments/assets/44631b34-444e-4df6-8c04-0e98407f14a3" />
<img width="1042" height="583" alt="johnC(4)" src="https://github.com/user-attachments/assets/79fba6f0-58cf-4357-bf26-bebe4e2d853a" />
<img width="949" height="516" alt="johnC(5)" src="https://github.com/user-attachments/assets/bf4e659e-7001-4970-98ce-fd72b41d67d0" />



### Resolution
- Diagnosed the issue as a broken charger.
- Replaced the charger, confirmed laptop charging successfully.
- Closed the ticket as **Resolved**, documenting the root cause.

<img width="929" height="854" alt="johnC(6)" src="https://github.com/user-attachments/assets/60a6312f-86d5-467b-9ad7-0a371dbe328b" />
<img width="933" height="474" alt="johnC(7)" src="https://github.com/user-attachments/assets/047b30fc-887e-42f1-87d8-3948acf548b9" />
<img width="903" height="401" alt="johnC(8)" src="https://github.com/user-attachments/assets/e94a7196-dda3-4441-9480-0f04fd858cbf" />


⚠️ **Note on Permissions:** Just like in Ticket 2, John should have had reply permissions here too. I only noticed it too late, which limited him to internal notes.

**Reflection:** Severity levels matter. A CFO’s laptop was treated as an Emergency, and I resolved it quickly. This emphasized the need for accurate prioritization and proactive permission checks.

---



---

## ✅ Reflections and Future Plans
Looking back at this project, I can see how much ground I covered. I went from simply creating tickets to fully managing their lifecycle—updating properties, assigning teams, escalating when necessary, and resolving issues with clear documentation. I also experienced first-hand how permissions and roles can affect communication between agents and end users.

For myself, this project shows that I am capable of using a ticketing system like osTicket in a professional setting. I know how to properly classify, prioritize, and close tickets while keeping user communication in mind.

### Future Learning Goals
- Explore the **email integration** feature more deeply so I can simulate real-world notifications and user responses.  
- Practice setting up **automation and SLA rules** to better understand how escalations can be enforced without manual changes.  
- Learn more about **reporting and metrics** so I can demonstrate how ticket data translates into performance insights.  
- Continue to redo this lab until every step feels natural and repeatable—building my technical intuition further.  
- Practice handling **ticket intake through multiple channels** (phone, chat, email, web forms, even in-person requests) to simulate real-world help desk conditions.  

**Personal Note:** This write-up is not just practice; it’s a showcase for future employers and teammates. It reflects both my technical ability and my commitment to documenting work clearly and professionally.
