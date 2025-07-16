<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Role
- Set Up Department
- Create Teams
- Manage Ticket Creation Settings
- Add Agents and Users
- Define SLAs
- Create Help Topics

<h1>Configuration Steps</h1>

<p>
<h2>Access osTicket Admin Panel</h2>

Admin Login URL: http://localhost/osTicket/scp/login.php
End User URL: http://localhost/osTicket
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Configure Roles</h2>

Path: Admin Panel -> Agents -> Roles

Example: Create a Supreme Admin role with full permissions.
Why: Restrict/modify access for other roles.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Set Up Departments</h2>

Path: Admin Panel -> Agents -> Departments

Example:
SysAdmins (Full access to technical tickets)
Support (Basic ticket visibility)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Create Teams</h2>

Path: Admin Panel -> Agents -> Teams

Example:
Online Banking (Agents from SysAdmins + Support)
Why: Collaborate across departments for specific issues.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Ticket Creation Settings</h2>

Path: Admin Panel -> Settings -> User Settings

Action:
UNCHECK: "Allow unregistered users to create tickets"
ENABLE: "Require registration/login to create tickets"
Why: Prevent spam and track users.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Add Agents (Workers)</h2>

Path: Admin Panel -> Agents -> Add New

Examples:
Lerone (Department: SysAdmins)
Leona (Department: Support)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Add Users (Customers)</h2>

Path: Agent Panel -> Users -> Add New

Examples:
Lerone (Email: Leona@example.com)
Leona (Email: Leona@example.com)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Configure SLAs</h2>

Path: Admin Panel -> Manage -> SLA

Examples:
SLA Plan	Grace Period	Schedule
Sev-A	1 hour	24/7
Sev-B	4 hours	24/7
Sev-C	8 hours	Business Hours (9AM-5PM)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Create Help Topics</h2>

Path: Admin Panel -> Manage -> Help Topics

Examples:
Business Critical Outage
Personal Computer Issues
Password Reset
Equipment Request
</p>
<br />
