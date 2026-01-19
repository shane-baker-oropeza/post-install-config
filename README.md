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
<img width="970" height="777" alt="Screenshot 2026-01-19 080116" src="https://github.com/user-attachments/assets/c14370bf-3466-455f-a95b-de888febbaaa" />

</p>
<br />

<p>
<img width="658" height="282" alt="Screenshot 2026-01-19 080127" src="https://github.com/user-attachments/assets/948193d1-a3ad-48b5-b762-0087f3c7f4a0" />

</p>
<br />

<p>
<img width="652" height="396" alt="Screenshot 2026-01-19 080147" src="https://github.com/user-attachments/assets/869b1f4e-b10e-4963-88af-17268717f9c2" />

</p>
<br />

<p>
<img width="977" height="603" alt="Screenshot 2026-01-19 080218" src="https://github.com/user-attachments/assets/6d7118c8-9864-4019-b901-7391d8b6dbd4" />

</p>
<br />

<p>
<img width="969" height="598" alt="Screenshot 2026-01-19 080327" src="https://github.com/user-attachments/assets/306a9093-94a2-4736-8a4e-93e62f30f315" />

</p>
<br />

<p>
<img width="974" height="464" alt="Screenshot 2026-01-19 080427" src="https://github.com/user-attachments/assets/ebec6750-dfeb-41c5-9a0b-97cfdafa9e66" />

</p>
<br />

<h3>Step 7: Configure Users (Customers)</h3> 

**Add the individuals who will be requesting help**

- Path: Agent Panel -> Users -> Add New
- Task: Create Karen

</p>
<br />

<p>
<img width="994" height="392" alt="Screenshot 2026-01-19 080638" src="https://github.com/user-attachments/assets/6b6782ba-a390-4d03-b2c4-62e52e6c3723" />

</p>
<br />

<p>
<img width="991" height="376" alt="Screenshot 2026-01-19 080651" src="https://github.com/user-attachments/assets/729d9d21-9841-4292-9fed-88b34994569e" />

</p>
<br />

<p>
<img width="660" height="402" alt="Screenshot 2026-01-19 080746" src="https://github.com/user-attachments/assets/99c3c60b-0ee7-448c-9478-80702c3a5d06" />

</p>
<br />

<p>
<img width="978" height="430" alt="Screenshot 2026-01-19 080802" src="https://github.com/user-attachments/assets/69ed316b-3013-4a88-888a-31a199d98c19" />

</p>
<br />

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
<img width="987" height="851" alt="Screenshot 2026-01-19 080952" src="https://github.com/user-attachments/assets/5c04c520-2bf8-4d2c-82f2-2e71335431a6" />

</p>
<br />

<p>
<img width="981" height="486" alt="Screenshot 2026-01-19 081002" src="https://github.com/user-attachments/assets/e7a30698-4ce6-4ebb-90fa-7e6385d8ec16" />

</p>
<br />

<p>
<img width="992" height="376" alt="Screenshot 2026-01-19 081011" src="https://github.com/user-attachments/assets/536497c2-a22e-4fad-9fc9-7cbd001ed005" />

</p>
<br />

<p>
<img width="974" height="725" alt="Screenshot 2026-01-19 081059" src="https://github.com/user-attachments/assets/4fa23e61-7312-47b9-86ba-64a5255abfa1" />

</p>
<br />

<p>
<img width="981" height="434" alt="Screenshot 2026-01-19 081118" src="https://github.com/user-attachments/assets/ac9e8d09-3678-45fc-ba76-22fe2b60b8d1" />

</p>
<br />

<p>
<img width="981" height="719" alt="Screenshot 2026-01-19 081141" src="https://github.com/user-attachments/assets/ae070060-a669-46b3-a0ca-c78cb4c8d1d5" />

</p>
<br />

<p>
<img width="974" height="463" alt="Screenshot 2026-01-19 081257" src="https://github.com/user-attachments/assets/1798aff1-ceed-46d4-8786-56eef5fe55c5" />

</p>
<br />

<p>
<img width="978" height="726" alt="Screenshot 2026-01-19 081357" src="https://github.com/user-attachments/assets/a5404560-f70a-4c2f-a4b2-7a9a185870ac" />

</p>
<br />

<p>
<img width="975" height="483" alt="Screenshot 2026-01-19 081333" src="https://github.com/user-attachments/assets/dc1d2506-983d-4396-9c10-578da16c47ab" />

</p>
<br />

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
<img width="970" height="489" alt="Screenshot 2026-01-19 081559" src="https://github.com/user-attachments/assets/3548dc3a-9ead-47ff-947d-cb4e73d1eae4" />

</p>
<br />

<p>
<img width="984" height="694" alt="Screenshot 2026-01-19 081714" src="https://github.com/user-attachments/assets/fdf5edbf-1bfc-40e7-95f6-c61d08040eb2" />


</p>
<br />

<p>
<img width="986" height="697" alt="Screenshot 2026-01-19 081633" src="https://github.com/user-attachments/assets/9eb34df0-0683-4bbd-b65b-af325a2565a0" />

</p>
<br />

<p>
<img width="984" height="694" alt="Screenshot 2026-01-19 081714" src="https://github.com/user-attachments/assets/d7dbbb52-682f-452e-b8de-1dd9ee06c1b6" />

</p>
<br />

<p>
<img width="974" height="699" alt="Screenshot 2026-01-19 081753" src="https://github.com/user-attachments/assets/85cd83da-de37-45db-89c4-f6cdb6583d8d" />

</p>
<br />

<p>
<img width="984" height="694" alt="Screenshot 2026-01-19 081714" src="https://github.com/user-attachments/assets/d9727875-db2f-44fd-ac7e-49346892f572" />

</p>
<br />

<p>
<img width="983" height="706" alt="Screenshot 2026-01-19 082135" src="https://github.com/user-attachments/assets/bbdde669-6c5a-4b1b-afda-92339f4d8462" />

</p>
<br />

<p>
<img width="966" height="702" alt="Screenshot 2026-01-19 082219" src="https://github.com/user-attachments/assets/fa591bdc-36c9-4a3a-9aa2-65ff1b392781" />

</p>
<br />

<p>
<img width="990" height="701" alt="Screenshot 2026-01-19 082248" src="https://github.com/user-attachments/assets/350322b6-3e6b-4560-b721-e599a933c16c" />

</p>
<br />

<p>
<img width="975" height="691" alt="Screenshot 2026-01-19 082316" src="https://github.com/user-attachments/assets/06975cb3-0336-4cc6-b7ae-78eac7fa27f4" />

</p>
<br />

<p>
<img width="977" height="693" alt="Screenshot 2026-01-19 082339" src="https://github.com/user-attachments/assets/909af91f-f3a8-45c6-bf72-cdacb9dfb5bf" />

</p>
<br />

<p>
<img width="977" height="711" alt="Screenshot 2026-01-19 082356" src="https://github.com/user-attachments/assets/8831b500-1bf4-4cb6-adf0-8416b02788f3" />
>
</p>
<br />


