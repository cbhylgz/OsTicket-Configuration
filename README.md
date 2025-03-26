<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Post-Installation Configuration</h1>

<h2>Description</h2>
In this guide, I will be configuring osTicket. This will allow it to run as it should so that it can be used properly as a ticketing system. The configuration will involve creating multiple agents and giving them specific departments, roles, and permissions. On top of that, I will also create SLA (Service Level Agreement) configuration, help topics, and users, all to help simulate an average day at the IT help desk.<br/>
<br/>

This project is a continuation of the [osTicket: Prerequisites and Installation](https://github.com/cbhylgz/OsTicket-Installation) project.
<br />


<h2>Environments and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Virtual Machines</b>
- <b>Remote Desktop Connection</b>
- <b>osTicket</b>


<h2>Operating Systems Used </h2>

- <b>Windows 10</b>

<h2>Steps to Take:</h2>

<p align="center">
Connect to the VM, and in osTicket navigate to the Admin Panel by clicking "Admin Panel" located in orange at the top right of the page: <br/>
<img src="https://i.imgur.com/uPKWaIt.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Now, let's begin configuring Roles. Go to the "Agents" tab and click on "Roles", and enter a role name. For this example, I chose 'Supreme Admin':  </br>
<img src="https://i.imgur.com/8RirX8T.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Don't click Add Role just yet-- if you do, you'll get an error message. What you'll want to do next is go to the Permissions tab and check all the boxes in the Tickets, Tasks, and Knowledgebase tab. NOW you can click Add Role:  </br>
<img src="https://i.imgur.com/nCkesTr.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Set up departments by clicking on Departments, located within the Agents tab:  <br/>
<img src="https://i.imgur.com/UK22n7v.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Click Add New Department, and then name the Department System Administrators (or SysAdmins, as shown here):  <br/>
<img src="https://i.imgur.com/MVnBg9A.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Now, let's create a team. Click "Teams" located within the Agents tab, click "Add New Teams", and then name it "Level II Support" before creating it:  <br/>
<img src="https://i.imgur.com/VGfj8an.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Hover over the Settings tab, and click Users. Under "Authentication Settings" make sure "Require registration and login to create tickets" is unchecked:  <br/>
<img src="https://i.imgur.com/psqfGdx.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
You can't have a team without individuals. That's where the agents come in. To create the help desk workers (AKA the agents), go back to "Agents" and select the Agents tab. Click Add New Agents, then fill out the name, email, and username: <br/>
<img src="https://i.imgur.com/TEjuRDr.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Don't forget to set which Department and Role they're in. For Jane here, I put her in the SysAdmin department and gave her the Supreme Admin role. Finally, I set her on the Level II Support Team:  <br/>
<img src="https://i.imgur.com/hCz8X1w.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
<img src="https://i.imgur.com/mILIUWS.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Click on "Set Password" and give Jane a password. Be sure to remember it for later, or keep track of it. Uncheck the "Send the agent a password reset email" and "Require password change at next login" boxes:  </br>
<img src="https://i.imgur.com/xBfR7gA.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Create one more agent. This time, however, put them in the Support department:  </br>
<img src="https://i.imgur.com/cqJfc9s.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Tickets are made for all types of technical issues, but typically, they're made when customers (Users, in this case) need assistance. To create a User, click 'Agent Panel' on the top right (You're on the Admin Panel if you see Agent Panel on the top right, and vice versa. Remember this!), click Users, then Add User. Put in the email and name of the User, and then click Add User one more time:  </br>
<img src="https://i.imgur.com/eeuQ4a6.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Add one more with the same steps:  </br>
<img src="https://i.imgur.com/sK0EgpM.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Now, it's time to configure SLA (Service Level Agreement) plans. Go back to the Admin Panel, click Manage, and then SLA. After that, click Add New SLA Plan and make three SLAs, each with their own individual severities, grace periods, and schedules. I've provided three of my own examples down below:  </br>
<img src="https://i.imgur.com/fFmQkrY.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
<img src="https://i.imgur.com/YqCektT.png" height ="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
<img src="https://i.imgur.com/c3oXH1y.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />
Finally, go to the "Help Topics" tab (which is under Manage), and create four help topics by clicking Add New Help Topic. Their titles are, in no specific order, "Password Reset", "Business Critical Outage", "Equipment Request", and "Personal Computer Issues". All of them must have the settings shown below:  </br>
<img src="https://i.imgur.com/V2fhutA.png" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />
<br />

<h2>osTicket Setup Complete!</h2>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
