<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Differentiate between Admin Panel and Agent Panel
- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

**You will need these 2 links in order to access osTicket for the lab**
- Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- End Users osTicket URL: http://localhost/osTicket

**Remote desktop into your Windows 10 virtual machine and log into osTicket with the Admin link above**


<h3>Step 1: Distinguish Agent Panel vs. Admin Panel</h3>

**Understand the difference between the two interfaces** 

- The Admin Panel is used for system-wide configuration, while the Agent Panel is where workers manage tickets and users. 
- Action: Locate the toggle button or link to switch between panels.
<br />

**This is the AGENT Panel**

<p>
<img width="1446" height="502" alt="Screenshot 2026-01-19 074206" src="https://github.com/user-attachments/assets/5615a1b1-b631-4dd5-b85e-234fc16bf14c" />

</p>
<br />

**This is the ADMIN Panel**

<p>
<img width="959" height="904" alt="Screenshot 2026-01-19 074311" src="https://github.com/user-attachments/assets/d6a0807b-57d5-4a76-8b3a-8bcf6615954a" />

</p>
<br />

<h3>Step 2: Configure Roles (Permission Grouping)</h3>  

**Roles define what actions an agent can perform (e.g., delete tickets, edit threads)**

- Path: Admin Panel -> Agents -> Roles
- Task: Create a Supreme Admin role with all permissions enabled.

</p>
<br />

<p>
<img width="990" height="430" alt="Screenshot 2026-01-19 074436" src="https://github.com/user-attachments/assets/f56a9bf0-c7ef-4dc1-838b-4c55d539698e" />

</p>
<br />

<p>
<img width="983" height="439" alt="Screenshot 2026-01-19 074448" src="https://github.com/user-attachments/assets/86f3b566-0e27-44c6-9d72-489d7506911d" />

</p>
<br />

<p>
<img width="980" height="636" alt="Screenshot 2026-01-19 074558" src="https://github.com/user-attachments/assets/82512946-c197-46ee-9605-a8520735917b" />


</p>
<br />

<p>
<img width="979" height="769" alt="Screenshot 2026-01-19 074711" src="https://github.com/user-attachments/assets/78da4f66-985d-4946-a204-1e2bcf822666" />

</p>
<br />

<p>
<img width="980" height="775" alt="Screenshot 2026-01-19 074618" src="https://github.com/user-attachments/assets/4b4a6613-2cbd-4167-8c6e-b2aa16086ba0" />

</p>
<br />

<h3>Step 3: Configure Departments (Ticket Visibility)</h3> 

**Departments control which tickets agents can see based on their specialty**

- Path: Admin Panel -> Agents -> Departments
- Task: Create a SysAdmins department.

</p>
<br />

<p>
<img width="969" height="409" alt="Screenshot 2026-01-19 074751" src="https://github.com/user-attachments/assets/3aa93aaf-9edb-4e84-b376-14659434423c" />

</p>
<br />

<p>
<img width="981" height="410" alt="Screenshot 2026-01-19 074808" src="https://github.com/user-attachments/assets/b254dc31-03ed-45ea-8a2c-0f6d9d381d8f" />

</p>
<br />

<p>
<img width="977" height="886" alt="Screenshot 2026-01-19 074839" src="https://github.com/user-attachments/assets/b0506b51-a050-457e-b792-c843395816f8" />

</p>
<br />

<p>
<img width="975" height="889" alt="Screenshot 2026-01-19 074935" src="https://github.com/user-attachments/assets/c90f45c5-0cca-4f24-b907-526a5a67082c" />

</p>
<br />

<p>
<img width="994" height="848" alt="Screenshot 2026-01-19 074957" src="https://github.com/user-attachments/assets/72fdc221-5205-4cf9-bd5f-f89a6204eba9" />

</p>
<br />

<p>
<img width="980" height="425" alt="Screenshot 2026-01-19 075020" src="https://github.com/user-attachments/assets/39d91236-fc93-4f91-9e71-d7bb12498773" />

</p>
<br />

<h3>Step 4: Configure Teams</h3> 

**Teams allow you to group agents from different departments to work on specific projects or issues**

- Path: Admin Panel -> Agents -> Teams
- Task: Create an Online Banking team.

</p>
<br />

<p>
<img width="975" height="398" alt="Screenshot 2026-01-19 075030" src="https://github.com/user-attachments/assets/9d5f04c1-edfe-4bdb-a9fb-20feaf664fe5" />

</p>
<br />

<p>
<img width="979" height="368" alt="Screenshot 2026-01-19 075041" src="https://github.com/user-attachments/assets/0717e018-04de-4ecb-85cc-c7a8c136e2c6" />

</p>
<br />

<p>
<img width="982" height="736" alt="Screenshot 2026-01-19 075102" src="https://github.com/user-attachments/assets/e2b4c7fb-c78d-46a9-8f34-37d45c8395a9" />

</p>
<br />

<p>
<img width="986" height="750" alt="Screenshot 2026-01-19 075119" src="https://github.com/user-attachments/assets/ed4700c6-399d-4a87-b3dc-344d6cc08961" />

</p>
<br />

<p>
<img width="978" height="407" alt="Screenshot 2026-01-19 075143" src="https://github.com/user-attachments/assets/773cb9b4-1ba5-44e9-bd88-bacdd0e57ddb" />

</p>
<br />

<h3>Step 5: Set User Registration Requirements</h3>  

**Decide if the system is open to the public or restricted to registered users**

- Path: Admin Panel -> Settings -> User Settings
- Task: UNCHECK the box for "Registration Required" to allow anyone to create tickets, or leave it checked if you require login.
</p>
<br />

<p>
<img width="977" height="911" alt="Screenshot 2026-01-19 075301" src="https://github.com/user-attachments/assets/cdf12cc1-89c6-41e8-b043-4f8c47505d1b" />

</p>
<br />

<p>
<img width="975" height="750" alt="Screenshot 2026-01-19 075315" src="https://github.com/user-attachments/assets/2ccc8117-661d-4148-91a6-e032edb3a4db" />

</p>
<br />

<p>
<img width="558" height="61" alt="Screenshot 2026-01-19 075403" src="https://github.com/user-attachments/assets/c345f87e-72b3-4e41-9a5a-a494e9baffd2" />

</p>
<br />

<h3>Step 6: Configure Agents (Workers)</h3> 

**Add the staff members who will be resolving the tickets**

- Path: Admin Panel -> Agents -> Add New
- Task: Create Jane (assigned to SysAdmins) and John (assigned to Support).

</p>
<br />

<p>
<img width="981" height="414" alt="Screenshot 2026-01-19 075449" src="https://github.com/user-attachments/assets/67be6a24-7d84-4704-887e-aae95c41fcfc" />

</p>
<br />

<p>
<img width="980" height="796" alt="Screenshot 2026-01-19 075501" src="https://github.com/user-attachments/assets/4202e84f-8fb5-4534-8afa-2f60ef641def" />

</p>
<br />

<p>
<img width="982" height="854" alt="Screenshot 2026-01-19 075805" src="https://github.com/user-attachments/assets/b69212d4-f938-4291-acc8-bf86f169c24f" />


</p>
<br />

<p>
<img width="663" height="277" alt="Screenshot 2026-01-19 075829" src="https://github.com/user-attachments/assets/d3c6f0d7-d3b2-436f-9c94-a28f0d05af99" />

</p>
<br />

<p>
<img width="663" height="409" alt="Screenshot 2026-01-19 075853" src="https://github.com/user-attachments/assets/b28080f2-fe94-4a3d-be9d-47b9811d9f5d" />

</p>
<br />

<p>
<img width="975" height="390" alt="Screenshot 2026-01-19 080008" src="https://github.com/user-attachments/assets/1ace4e43-43db-46af-a5a6-162da8f8b6b1" />

</p>
<br />

<p>
<img width="980" height="432" alt="Screenshot 2026-01-19 080020" src="https://github.com/user-attachments/assets/00ff1ce2-ac06-459d-be36-98b6f5c4ff9b" />

</p>
<br />

<p>
<img width="981" height="492" alt="Screenshot 2026-01-19 080442" src="https://github.com/user-attachments/assets/5c2c7abc-4220-4a03-9045-6affe5b4e308" />

</p>
<br />

<p>
<img width="983" height="428" alt="Screenshot 2026-01-19 080045" src="https://github.com/user-attachments/assets/ab484570-ae6c-423b-b69b-ee6dfd044c04" />

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />




<p>

<h3>Step 7: Configure Users (Customers)</h3> 

**Add the individuals who will be requesting help**

- Path: Agent Panel -> Users -> Add New
- Task: Create Karen and Ken.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<p>

<h3>Step 8: Configure Service Level Agreements (SLA)</h3>  

**Define the expected response and resolution times for tickets**

- Path: Admin Panel -> Manage -> SLA
- Task: Create the following:
  1.  Sev-A: 1-hour Grace Period, 24/7 Schedule.
  2.  Sev-B: 4-hour Grace Period, 24/7 Schedule.
  3.  Sev-C: 8-hour Grace Period, Business Hours.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<p>

<h3>Step 9: Configure Help Topics</h3>  

**Set up the categories users select when submitting a ticket to ensure proper routing**

- Path: Admin Panel -> Manage -> Help Topics
- Task: Add topics for:
  
  1.  Business Critical Outage
  2.  Personal Computer Issues
  3.  Equipment Request
  4.  Password Reset
  5.  Other
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
