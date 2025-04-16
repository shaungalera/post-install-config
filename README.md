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

- Acknowledge the difference between the Agent Panel and Admin Panel.
- Configure Roles to define permissions for agents.
- Set up Departments to group tickets by areas of responsibility.
- Create Teams to pull agents from multiple departments.
- Configure user settings to allow or restrict ticket creation.
- Add Agents (workers) and Users (customers).
- Set up Service Level Agreements (SLAs) for ticket response times.
- Create Help Topics for users to categorize their tickets.

<h2>Configuration Steps</h2>

<h3>1.) Acknowledge Agent Panel vs Admin Panel</h3>

- The **Agent Panel** is used by agents to work on tickets.
- The **Admin Panel** is used to manage system settings, configurations, and permissions.

<h3>2.) Configure Roles</h3>

Navigate to **Admin Panel -> Agents -> Roles**.
Add a new role called **Supreme Admin**.
- Define permissions for agents based on the role they will have. In this lab, we will give permissions for the Tickets, Tasks, and Knowledgebase sections.

![image](https://github.com/user-attachments/assets/f35bc5e4-c261-4dac-88b3-f993077ccb75)
![image](https://github.com/user-attachments/assets/e9edc228-1bc3-4700-8467-c34e2709784a)
![image](https://github.com/user-attachments/assets/0e25a3d3-83d5-4f71-a2cd-d7cb37a41084)

<h3>3.) Configure Departments</h3>

- Navigate to **Admin Panel -> Agents -> Departments**.
- Add a new department called **SysAdmins**.
  - Use departments to control ticket visibility and assign areas of responsibility (e.g., Help Desk, SysAdmins, Networking).

![image](https://github.com/user-attachments/assets/795b04ed-5e3f-4ccd-8809-2fbdc4b39982)

<h3>4.) Configure Teams</h3>

- Navigate to **Admin Panel -> Agents -> Teams**.
- Create a new team called **Online Banking**.
  - Pull agents from different departments to form specialized teams.
 
![image](https://github.com/user-attachments/assets/fda3ccdc-1e28-4094-a89a-98f0a117cfba)

<h3>5.) Allow Anyone to Create Tickets</h3>

- Navigate to **Admin Panel -> Settings -> User Settings**.
- Uncheck **Require registration and login to create tickets** to enforce ticket creation by anyone.
- Enable **Public - Anyone can register** to disable requiring users to register and log in before creating tickets.

![image](https://github.com/user-attachments/assets/503a33ee-ca11-4a6b-9e52-7eff9b7e8b7d)

<h3>6.) Configure Agents (Workers)</h3>

- Navigate to **Admin Panel -> Agents -> Add New**.
- Add agents with the following details:
  - **Jane**: Assigned to the **SysAdmins** department.
  - **John**: Assigned to the **Support** department.

![image](https://github.com/user-attachments/assets/f6281848-c101-4ecc-8bc9-db0d3ba64c52)

You can choose to set their password or send the agent a password reset email.

![image](https://github.com/user-attachments/assets/907fbc14-b019-4915-8de0-521198eb70c8)
![image](https://github.com/user-attachments/assets/0b8ac0b3-13cc-4389-bc04-f726d621b2bf)
![image](https://github.com/user-attachments/assets/bb86f39a-ddc1-49a4-b778-0004f6b13623)
![image](https://github.com/user-attachments/assets/24862b99-9fea-42ff-9775-e723eda9135e)
![image](https://github.com/user-attachments/assets/ee7c8118-d758-42ca-8925-7929a3073f40)
![image](https://github.com/user-attachments/assets/1acf0a10-f4da-4053-964a-0f86f67196df)

<h3>7.) Configure Users (Customers)</h3>

- Navigate to **Agent Panel -> Users -> Add New**.
- Add users with the following details:
  - **Karen**
  - **Ken**

![image](https://github.com/user-attachments/assets/02783eec-5b09-445b-92f4-1f5be8cd7b9c)

<h3>8.) Configure SLA (Service Level Agreements)</h3>

- Navigate to **Admin Panel -> Manage -> SLA**.
- Add the following SLAs:
  - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.
  - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.
  - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.
 
![image](https://github.com/user-attachments/assets/c169353a-63ad-4a41-b021-0da963832245)
![image](https://github.com/user-attachments/assets/7bc6d45b-e139-421c-b1c3-c3216aeeecfd)
![image](https://github.com/user-attachments/assets/2108c7c6-8437-4ef7-a0f5-9b925017983f)
![image](https://github.com/user-attachments/assets/e8d8be12-02a9-4bd3-8c9d-4fda83f4722c)

<h3>9.) Configure Help Topics</h3>

- Navigate to **Admin Panel -> Manage -> Help Topics**.
- Add the following help topics for users to select when creating a ticket:
  - **Business Critical Outage**
  - **Personal Computer Issues**
  - **Equipment Request**
  - **Password Reset**
  - **Other**

![image](https://github.com/user-attachments/assets/d873e863-5eb4-421f-b7bd-3f362582ce7d)
![image](https://github.com/user-attachments/assets/518798e0-d1b0-4f2a-ab55-a2c32eb0fbe4)
![image](https://github.com/user-attachments/assets/3a5f9e7b-f3d0-4366-87ee-a343adecfe5a)
![image](https://github.com/user-attachments/assets/e87f656e-bc24-4b12-851a-dea3cc16e4b1)

<h2>Conclusion</h2>

By completing the post-installation configuration steps, you have successfully customized osTicket to suit your organization's requirements. You are now ready to start using osTicket to manage and resolve customer issues efficiently.
