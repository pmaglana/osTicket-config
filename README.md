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

<h3>Configure Roles (Add/Remove permissions)</h3>
               
- We are going to add "Supreme Admin" as a new role that grants a user full access to the sytem.
     - Admin Panel -> Agents -> Roles -> click Add New Role.
               <img width="959" height="380" alt="post1" src="https://github.com/user-attachments/assets/1de466d6-282a-47a7-9ccb-83aa63c3a180" />
               <img width="957" height="568" alt="post2" src="https://github.com/user-attachments/assets/240fd404-db09-47c4-a208-16baae11bccf" />

     - Under Permission tab, check all the boxes from Tickets, Tasks and Knowledgebase tabs and hit "Add Role".
               <img width="956" height="406" alt="post3" src="https://github.com/user-attachments/assets/77a52a34-50ea-49ef-9d98-cc0118e73874" />
               <img width="952" height="441" alt="post4" src="https://github.com/user-attachments/assets/8414450b-bf2f-492a-a022-a376caa7d774" />

       
      


Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking

Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)

Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other

