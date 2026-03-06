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
     <img src="images/post1.png"  >
               
- Adding "Supreme Admin" as a new Role that grants a user full access to the sytem.
     - Admin Panel > Agents > Roles > click Add New Role.
          <img src="images/post2.png"  >
             
     - Under Permission tab, check all the boxes from Tickets, Tasks and Knowledgebase tabs and hit "Add Role".
          <img src="images/post3.png">
          <img src="images/post4.png" >
              
<h3>2. Departments: Allows different level of Ticket Visibility. ie. Help Desk vs SysAdmins vs Networking</h3>
     <img src="images/dept.png"  >  
                 
- Adding "SysAdmins" as a new Department. 
     - Admin Panel > Agents > Department > Select "Top Level Department" as Parent, type in "SysAdmins" under Name > hit Add New Role.</br>
          <img src="images/dept1.png">
          <img src="images/dept2.png"  >
                    
<h3>3. Teams: Allows user to pull Agents from different Departments to form a new team. </h3>

- Let's create a new team and name it "Online Banking".
     - Admin Panel > Agents > Teams > click Add New Team
          <img src="images/teams.png"  >
     - Type "Online Banking" under Name, then click Create Team. *(We will add Members and Team Lead at the later part of this activity.)*
          <img src="images/teams1.png"  >
          
<h3>4. User Settings: This particular setting will allow anyone to create tickets. </h3>

- UNCHECK Require registration and loging to create tickets.
     - Admin Panel > Settings > User Settings > Uncheck Registration Required > Save Changes.
          <img src="images/settings.png"  >

<h3>5. Agents: Adding new Agents/employees. Use the Agent's credential and information below. </h3>

- Name: Jane Doe | Email: jane@eatech.com | Department: SysAdmins | Role: Supreme Admin | Team: Online Banking | Username: jane | Password: Password1
- Name: John Doe | Email: john@eatech.com | Department: Support | Role: View only | Team: - | Username: john | Password: Password1
  
- To add new Agents go to...
     - Admin Panel > Agents > Add New
          <img src="images/agent.png" >
     - Under Account tab, enter the agent's personal information, including the username and password.
          <img src="images/agent1.png"  >
          <img src="images/agent4.png" >
     - From the Access tab, choose SysAdmins and Supreme Admin from Primary Dept.
          <img src="images/agent2.png" >
     - And at the Teams tab, choose SysAdmins and Supreme Admin from Primary Dept.
           <img src="images/agent3.png" >          
     - Create another Agent and use the following details and credentials:



<h3>6. Configure Users/Customer</h3>

- Make sure you are on the Agent panel then, follow the steps below to add a User.</br>
     Agent Panel -> Users -> Add New</br>
     <img src="images/user.png">          
     <img src="images/user1.png">          


<h3>7. Configuring Service Level Agreement. SLA's are defined by the grace period given to a ticket depending on it's severity.</h3>

To configure SLA's go to Admin Panel > Manage > SLA > After entering information on the required textbox, click Add Plan. Use the three level of SLA's below.

   - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
   - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
   - Sev-C (Grace Period: 8 hours, Business Hours)</br>
   
     <img src="images/SLA.png">          
     <img src="images/SLA1.png"> 
     
<h3>8. Configure Help Topics (For when users create a ticket).</h3>

To configure Help Topics go to Admin Panel > Manage > Help Topics >  Use the information below to add Help Topics.

   - Business Critical Outage
   - Personal Computer Issues
   - Equipment Request
   - Password Reset
   - Other
   
     <img src="images/help.png">          
     <img src="images/help1.png"> 

<h2>Finishing Up</h2>
<h3>That Concludes our initial setup for osTicket. In our next lab, we'll Ticket Lifecycle (Ticketing simulation).</h3>


<sub>For questions and concerns, please reach out to paulo@maglana.com*</sub>







