<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://youtu.be/knrn3dqGj70)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>If you need help installing osTicket follow my tutorial here</h2>

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents
- Configure Users
- Configure Service Level Agreements(SLA)
- Configure Help topics

<h2>Configuration Steps</h2>

<h2>Configure Roles</h2>

In the admin panel
- Select the Agents tab -> Roles -> Add New Role
	- Name : Supreme Admin
	- Select Permissions tab and check every box under the "Tickets", "Tasks" and "Knowledgebase" section
- Select Add Role
<p>
<img src="https://i.imgur.com/5tVVX8e.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Configure Departments</h2>

- In the admin panel
- Select the Agents tab -> Departments -> Add New Department 
	- Name: System Administrators
- Select Create Deptartment 
<p>
<img src="https://i.imgur.com/9ZCvLxv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hYlBpT4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>	
	
<h2>Configure Teams</h2>

- In the admin panel
- Select the Agents tab -> Teams -> Add New Team
	- Name: Level II Support 
- Go to members tab and select yourself in "Select Agent" dropdown menu
- Select create team. 
<p>
<img src="https://i.imgur.com/90A9Thc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/LGfX8Dr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>	
	
<h2>Open Permissions to Allow Anyone to Create Tickets</h2>

 In the admin panel 
- Select the Settings -> User Settings
- Make sure box the "Registration Required: "Require registration and login to create tickets"is unchecked:  
<p>
<img src="https://i.imgur.com/JV6rpkd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>		
	
<h2>Configure Agents</h2>

-  In the admin panel 
- Select the Agents tab -> Add New Agents
	- Name: Jane Doe
	- Email : jane.doe@osticket.com
	- Username: jane.doe
	- Click set password and uncheck box that says "send the agent a password reset email
		- Set your password
		- uncheck "require password change at next login" box
		- set
<p>
<img src="https://i.imgur.com/3dO2yIQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/feSztGC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

- Select Access tab 
	- Under Primary Department 
		- Select department dropdown menu -> System Administrators
		- Select Role dropdown menu -> Supreme Admin
	- Extended Accesss 
		- Select Department -> Support -> Add -> Supreme Admin
- Select Teams tab
	- Select team dropdown menu -> Level II Support
	- Select Add
- Select Create	

<p>


</p>

- Create another agent named john and repeat the process again.
	- Follow same steps as above with some changes to Primary Department
		- Select department dropdown menu -> Support
		- Select Role dropdown menu -> View only
	- Extended Accesss 
		- Select Department -> Support -> Save Changes

<p>
<img src="https://i.imgur.com/5m4QbFO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/nn0JfQ6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



<h2>Configure Users</h2>

- In the Agent panel
- Select Users tab to create user
	- Email Address: Karen@osticket.com
	- Full Name - Karen Karen
	- Select Add User

<p align="center">
<img src="https://i.imgur.com/3P6AAAW.png" height="80%" width="80%" />

- Select user tab again to create another user
	- Email Address: Ken@osticket.com
	- Full Name - Ken Ken
	- Select Add User

<p align="center">
<img src="https://i.imgur.com/R9o7dbG.png" height="80%" width="80%" />


<h2>Configure Service Level Agreements(SLAs)</h2>

- In the admin panel 
- Select Manage tab -> SLA -> Add New SLA Plan 
	- Name: SEV-A 			
	- Grace Period: 1
	- Schedule dropdown menu: 24/7
	- Select Add Plan	
	
<p align="center">
<img src="https://i.imgur.com/v8A8WuT.png" height="80%" width="80%" /> <img src="https://i.imgur.com/8kG8Y7s.png" height="80%" width="80%" alt=/>
</p>

- Name: SEV-B
- Grace Period: 4
- Schedule dropdown menu: 24/7
- Select Add Plan
	
<p align="center">
<img src="https://i.imgur.com/XusprXO.png" height="80%" width="80%" />
</p>

- Name: SEV-C 
- Grace Period: 8
- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S Holidays
- Select Add Plan

<p align="center">
<img src="https://i.imgur.com/299PKRB.png" height="80%" width="80%" />
	

	
<h2>Configure Help Topics</h2>

- In the admin panel 
- Select Manage tab -> Help Topics -> Add New Help Topic 
	- Business Critical Outage
	- Personal Computer Issues
	- Equipment Request
	- Password Reset
- Select Add Topic for each topic

<p align="center">
<img src="https://i.imgur.com/fMpQIAB.png" height="80%" width="80%" />
<img src="https://i.imgur.com/eWf36p1.png" height="80%" width="80%" />

Done.
