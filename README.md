<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket Post-Installation Setup Guide</h1>

<h2>About this Project</h2>

In this project we will define the important function setup the necessary configuration needed in osTicket before we start creating and  solving mock tickets in the next part of this laboratory exercise.

<h2>Environment & Technology Used</h2>

- Microsoft Windows Virtual Machine 
- Remote Desktop
- osTicket

<h2>Prerequisites</h2>

- Admin/Analyst Login Page:
     http://localhost/osTicket/scp/login.php

- End Users osTicket URL:
     http://localhost/osTicket 

<h2>Getting Started</h2>

<h3>1. Roles: Here we can assign different Permission to different Roles.</h3>
     <img src="images/post1.png" width="75%" >
               
- Adding "Supreme Admin" as a new Role that grants a user full access to the sytem.
     - Admin Panel > Agents > Roles > click Add New Role.
          <img src="images/post2.png" width="75%" >
             
     - Under Permission tab, check all the boxes from Tickets, Tasks and Knowledgebase tabs and hit "Add Role".
          <img src="images/post3.png" width="75%" >
          <img src="images/post4.png" width="75%" >
              
<h2>2. Departments: Allows different level of Ticket Visibility. ie. Help Desk vs SysAdmins vs Networking</h2>
     <img src="images/dept.png" width="75%" >  
                 
- Adding "SysAdmins" as a new Department. 
     - Admin Panel > Agents > Department > Select "Top Level Department" as Parent, type in "SysAdmins" under Name > hit Add New Role.</br>
          <img src="images/dept1.png" width="75%" >
          <img src="images/dept2.png" width="75%" >
                    
<h2>3. Teams: Allows user to pull Agents from different Departments to form a new team. </h2>

- Let's create a new team and name it "Online Banking".
     - Admin Panel > Agents > Teams > click Add New Team
          <img src="images/teams.png" width="75%" >
     - Type "Online Banking" under Name, then click Create Team. *(We will add Members and Team Lead at the later part of this activity.)*
          <img src="images/teams1.png" width="75%" >
          
<h2>4. User Settings: This particular setting will allow anyone to create tickets. </h2>

- UNCHECK Require registration and loging to create tickets.
     - Admin Panel > Settings > User Settings > Uncheck Registration Required > Save Changes.
          <img src="images/settings" width="75%" >

<h2>5. Agents: Adding new Agents/employees. Use the Agent's credential and information below. </h2>

- Name: Jane Doe | Email: jane@eatech.com | Department: SysAdmins | Role: Supreme Admin | Team: Online Banking | Username: jane | Password: Password1
- Name: John Doe | Email: john@eatech.com | Department: Support | Role: View only | Team: - | Username: john | Password: Password1
  
- To add new Agents go to...
     - Admin Panel > Agents > Add New
          <img src="images/agent.png" width="75%" >
     - Under Account tab, enter the agent's personal information, including the username and password.
          <img src="images/agent1.png" width="75%" >
          <img src="images/agent4.png" width="75%" >
     - From the Access tab, choose SysAdmins and Supreme Admin from Primary Dept.
          <img src="images/agent2.png" width="75%" >
     - And at the Teams tab, choose SysAdmins and Supreme Admin from Primary Dept.
           <img src="images/agent3.png" width="75%" >          
     - Create another Agent and use the following details and credentials:



<h2>Configure Users/Customer</h2>
- Make sure you are on the Agent panel then, follow the steps below to add a User.
Agent Panel -> Users -> Add New
Karen
Ken

<h2>Configure SLA</h2>
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

<h2>Configure Help Topics (For when users create a ticket)</h2>
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other

