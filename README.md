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

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure: Roles, Departments, and Teams
- SLA Levels
- Agent Permissions
- User Access
- Basic Help Topics (Internal use only)


<h2>Configuration Steps</h2>

<p>
<img src="https://imgur.com/ypBQ1jf" height="80%" width="80%" alt="osTicket login"/>
</p>
<p>
Once all installation steps and requsites have been installed, login to osTicket at: http://localhost/osTicket/scp/login.php
</p>
<br />

<p>
<img src="https://imgur.com/jYA8H8a.png" height="80%" width="80%" alt="Admin panel"/>
</p>
<p>
From the main screen select the "Admin Panel" to start configuring osTicket.
</p>
<br />

<p>
<img src="https://imgur.com/Ht64bpf.png" height="80%" width="80%" alt="Add Roles"/>
</p>
<p>
Within Admin Panel, navigate to Agents -> Roles -> Add New Role. 
</p>
<br />

<p>
<img src="https://imgur.com/pqEtT8v.png" height="80%" width="80%" alt="Supreme Admin"/>
</p>
<p>
Create the role "Supreme Admin" and enable all permissions within the "Permissions" tab. Once configured, select "Add Role".
</p>
<br />

<p>
<img src="https://imgur.com/e78dMEu.png" height="80%" width="80%" alt="Add Department"/>
</p>
<p>
Navigate back to the main "Agents" tab and select Departments -> "Add New Department".
</p>
<br />

<p>
<img src="https://imgur.com/kQHIXHB.png" height="80%" width="80%" alt="SysAdmins"/>
</p>
<p>
No need to edit any settings, simply set name to "SysAdmins" and select "Create Dept".
</p>
<br />

<p>
<img src="https://imgur.com/xfBy5q5.png" height="80%" width="80%" alt="Create Team"/>
</p>
<p>
Back in main "Agents" tab, navigate to Teams -> "Add New Team".
</p>
<br />

<p>
<img src="https://imgur.com/63KMfKv.png" height="80%" width="80%" alt="Online Banking"/>
</p>
<p>
Create a new team with the name "Online Banking", select "Create Team".
</p>
<br />

<p>
<img src="https://imgur.com/TWNIjjS.png" height="80%" width="80%" alt="Add Agents"/>
</p>
<p>
Within main "Agents", Agents -> "Add New Agent". This is where you add team members that will access the osTicket program and be able to intract with tickets submitted to the system. For our purposes we will be creating two agents, one being support and one being an Administrator.
</p>
<br />

<p>
<img src="https://imgur.com/0K9gGRK.png" height="80%" width="80%" alt="New agent Credentials"/>
</p>
<p>
Create two Agents. 
First agent's credentials: 
Name: Jane Smith
Email: jane@email.com
Username: jane

Second agent's credentials:
Name: Jacob West
Email: jacob@email.com
Username: jacob

Follow next steps to set password and permissions for agent.
</p>
<br />

<p>
<img src="https://imgur.com/mEK729I.png" height="80%" width="80%" alt="Set Password"/>
</p>
<p>
Within the "Add New Agent" menu, select "Set Password" and uncheck "Send the agent a password reset email", Enter "Password1" for both boxes and agents. Also, uncheck "Require password change at next login" for ease of use. Once passwords match select "Set".
</p>
<br />

<p>
<img src="https://imgur.com/n6mawYC.png" height="80%" width="80%" alt="Agent Access">
</p>
<p>
Under the "Access" tab for agent Jane set: 
Department: SysAdmins 
Role: Supreme Admin

for agent Jacob:
Department: Support
Role: View only
</p>
<br />

<p>
<img src="https://imgur.com/VbMaiXy.png" height="80%" width="80%" alt="Agent Teams">
</p>
<p>
Under the "Teams" tab for agent Jane, select "Online Banking". Jacob will not be in a team. Once agent configuration is complete, select "Create".
</p>
<br />

<p>
<img src="https://imgur.com/ApvqKxf.png" height="80%" width="80%" alt="Create SLAs">
</p>
<p>
Open the "Manage" tab, navigate to SLA -> "Add New SLA Plan".
</p>
<br />

<p>
<img src="https://imgur.com/0DVS5Ar.png" height="80%" width="80%" alt="SLA Config">
</p>
<p>
Create three new SLA plans:
Plan "Sev-A":
Grace Period: 1 hour
Schedule: 24/7

Plan "Sev-B":
Grace Period: 4 Hours
Schedule: 24/7

Plan "Sev-C":
Grace Period: 8 Hours
Schedule: 24/5 (Business Hours)
</p>
<br />

<p>
<img src="https://imgur.com/dQgZ2Pg.png" height="80%" width="80%" alt="SLA List">
</p>
<p>
SLA plans should show up the same as displayed above.
</p>
<br />

<p>
<img src="https://imgur.com/pjj10qB.png" height="80%" width="80%" alt="Add Help Topics">
</p>
<p>
Navigate to Help Topics -> "Add New Help Topic".
</p>
<br />

<p>
<img src="https://imgur.com/nTNxi4P.png" height="80%" width="80%" alt="Help Topic Config">
</p>
<p>
Create five new help topics.
"Help Topic" -> "Parent Topic"
Business Critical outage ->  Report a Problem
Personal Computer Issues->  Report a Problem
Password Reset->  Report a Problem
Equipment Request-> General Inquiry
Other-> General Inquiry
No other settings need adjusted for the sake of this tutorial. 
</p>
<br />

<p>
<img src="https://imgur.com/zTdx9oF.png" height="80%" width="80%" alt="Complete Help Topics">
</p>
<p>
Verify that all help topics show up as displayed above.
</p>
<br />

<p>
<img src="https://imgur.com/1enADKu.png" height="80%" width="80%" alt="Agent Panel">
</p>
<p>
Navigate back to the "Agent Panel" on the top right of the screen. 
</p>
<br />

<p>
<img src="https://imgur.com/KAmsxY4.png" height="80%" width="80%" alt="New User">
</p>
<p>
Go to Users -> "Add User".
</p>
<br />

<p>
<img src="https://imgur.com/EkO8t2h.png" height="80%" width="80%" alt="">
</p>
<p>
Enter email and name (e.g., karen: karen@email.com), select "Add User".

This is the end of configuration for osTicket. In the next repository we will be utilizing everything we just made to make tickets and mock a typical ticket lifecycle.
</p>
<br />