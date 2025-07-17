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
<img width="2240" height="1260" alt="Image" src="https://github.com/user-attachments/assets/4d4ab7a8-4c91-490d-94b3-6b80d12233e1" />
</p>
<p>
<h2>Configure Roles</h2>

Path: Admin Panel -> Agents -> Roles

Example: Create a Supreme Admin role with full permissions.
Why: Restrict/modify access for other roles.
</p>
<br />

<p>
<img width="2240" height="1260" alt="Image" src="https://github.com/user-attachments/assets/46ec3d10-fe4d-47d9-956d-3069f2c2352b" />
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
<img width="942" height="489" alt="Image" src="https://github.com/user-attachments/assets/380e614f-9787-4f30-9ca8-8486a15b8036" />
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
<h2>Ticket Creation Settings</h2>

Path: Admin Panel -> Settings -> User Settings

Action:
UNCHECK: "Allow unregistered users to create tickets"
ENABLE: "Require registration/login to create tickets"
Why: Prevent spam and track users.
</p>
<br />

<p>
<h2>Add Agents (Workers)</h2>

Path: Admin Panel -> Agents -> Add New

Examples:
Lerone (Department: SysAdmins)
Leona (Department: Support)
</p>
<br />

<p>
<img width="941" height="943" alt="Image" src="https://github.com/user-attachments/assets/152c907e-6f12-4fb9-82e4-cd62715ec164" />
</p>
<p>
<h2>Add Users (Customers)</h2>

Path: Agent Panel -> Users -> Add New

Examples:
Ronaldo (Email: Ronaldo@example.com)
Messi (Email: Messi@example.com)
</p>
<br />

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
<img width="947" height="500" alt="Image" src="https://github.com/user-attachments/assets/8a8fca6c-b658-4514-a4ab-6c1200e1a235" />
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
<p>
<img width="946" height="678" alt="Image" src="https://github.com/user-attachments/assets/7fe11858-ee6a-4bce-9a61-cf4255a31f29" />
</p>
<br />
