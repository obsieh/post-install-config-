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

- Item 1: Secure Configuration Files
- Item 2:Remove Setup Files
- Item 3: Configure Admin Settings
- Item 4: Enable Necessary Plugins
- Item 5: Test the System

<h2>Configuration Steps</h2>

Step 1: Log In to osTicket

  ![image](https://github.com/user-attachments/assets/665fe04a-7880-449a-8f20-c6ba467c28d8)
  

</p>
<p>
To begin, log in to the system via the Admin/Analyst Login Page at http://localhost/osTicket/scp/login.php. This page provides access to administrative and ticket management features. End users can log in at http://localhost/osTicket to create and track tickets. Understanding the difference between these portals is key: the Admin Panel is for configuration, while the Agent Panel is for operational tasks.


</p>
<br />
Step 2: Define Roles and Departments

![image](https://github.com/user-attachments/assets/e2ff34d0-ef4b-4740-9939-27980c88f6de)

<p>
In the Admin Panel, create roles under Agents -> Roles to define permission levels for different types of agents, such as a Supreme Admin with full access. Set up departments under Agents -> Departments to organize agents and control ticket visibility. For instance, you can have separate departments for Help Desk, SysAdmins, and Networking to manage different areas of support.
</p>
<br />
Step 3: Configure Teams and Users

![image](https://github.com/user-attachments/assets/b5aa3878-e3ac-4c69-960f-a418f631099c)

<p>
Use Agents -> Teams in the Admin Panel to form cross-departmental teams for collaborative tasks, such as an Online Banking team. Add individual agents under Agents -> Add New, assigning them to specific departments. For example, Jane can be assigned to SysAdmins, while John is part of Support. Additionally, register users in Agent Panel -> Users -> Add New to manage customers, such as adding Karen and Ken as users who will submit tickets.
</p>
<br />
Step 4: Set SLAs and Help Topics

![image](https://github.com/user-attachments/assets/a7ac703d-1bd0-4df1-8ae9-ec1603cced44)

Define Service Level Agreements (SLAs) under Manage -> SLA to establish ticket response times. For example, Sev-A might have a 1-hour grace period with 24/7 coverage, while Sev-C could allow 8 hours during business hours. To streamline ticket creation, set up Help Topics under Manage -> Help Topics. Topics like Business Critical Outage, Password Reset, and Equipment Request make it easier for users to categorize their issues effectively.
