<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
This project involves a walkthrough on creating a simple Active Directory home lab using Oracle Virtualbox. By configuring and running the lab, you gain an understanding of how the service works, as well as the networking principles behind it. In this project, a server with the necessary networking settings and features will be set up, along with a script to generate 1000 users for demonstration purposes. The result will be tested in a separate environment acting as a client or user trying to login with their new credentials.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Oracle VM VirtualBox</b>
- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Windows 10 ISO</b> 
- <b>Server 19 ISO</b>

<h2>Project Walkthrough:</h2>

<p align="center">
1. This is the plan that is going to be followed throughout this project : <br/>
<img src="https://imgur.com/XyPL4NJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
2. Virtual Machines that are going to be used throughout this project have been created and uploaded:  <br/>
<img src="https://imgur.com/Zv0dZUg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
3. Installation of the Server 2019 vm:  <br/>
<img src="https://imgur.com/WuihVIM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
4. Server has started up:  <br/>
<img src="https://imgur.com/FmKYxTc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
5. Network Configuration:  <br/>
<img src="https://imgur.com/MLk6ZGZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
6. This adapter gave us an automatic IP address, therefore it can be used to connect to the internet:  <br/>
<img src="https://imgur.com/W1iIhkF.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
<br />
<br />
7. Following the diagram, the internal adapter was given the IP address of 172.16.0.1:  <br/>
<img src="https://imgur.com/cj4uHBx.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
<br />
<br />
8 Renaming this pc to DC (Domain Controller) for simplicity:  <br/>
<img src="https://imgur.com/KKAC8Pj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
9 This is the server manager which will be used to install all services and tools used thoughout this project:  <br/>
<img src="https://imgur.com/4sgg4pY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
10 Installation of Active Directory pt1:  <br/>
<img src="https://imgur.com/ME38stp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
11 Installation of Active Directory pt2:  <br/>
<img src="https://imgur.com/3an9byr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
12 Active Directory has been installed:  <br/>
<img src="https://imgur.com/d4OS0Ri.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<br />
13 Creation of an organisational unit for admin accounts:  <br/>
<img src="https://imgur.com/b7nye3n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
14 Instead of using the dedicated admin account, we are going to create our own admin account using our own credentials:  <br/>
<img src="https://imgur.com/2ZzH6r1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
15 An admin account with my name has been created:  <br/>
<img src="https://imgur.com/Ym70WkO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
16 Now we sign out of that admin account and log in to our new one with the new credentials:  <br/>
<img src="https://imgur.com/KPCkVuC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
17 Installation of Remote access pt1:  <br/>
<img src="https://imgur.com/ZPCwWnP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
18 Installation of Remote access pt2:  <br/>
<img src="https://imgur.com/AlF98Rd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
19 Select NAT to allow clients to connect to the internet using only one address:  <br/>
<img src="https://imgur.com/QVmGvx7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
21 Remote access is now enabled:  <br/>
<img src="https://imgur.com/BMtGAUg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
22 Installation of DHCP pt1:  <br/>
<img src="https://imgur.com/4KziuVK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
23 Installation of DHCP pt2:  <br/>
<img src="https://imgur.com/lCAKzd7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
24 Installation of DHCP is complete, this will allow computers/devices on the network to automatically recive an IP address:  <br/>
<img src="https://imgur.com/cbymAH6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
25 Creation of a new scope, this will be the range of IP addresses that are available within DHCP:  <br/>
<img src="https://imgur.com/giHhIVc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
26 This is going to be the range:  <br/>
<img src="https://imgur.com/hPHxhYP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
27 This is the lease, so the amount of time availble for an IP address before it expires on a used device:  <br/>
<img src="https://imgur.com/AnDxipj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
28 The IP address should be the same one assigned to the server, since it's going to act as a gateway for clients to forward traffic to the internet:  <br/>
<img src="https://imgur.com/d6o97Xu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
29 IPv4 turned green, therefore it worked:  <br/>
<img src="https://imgur.com/33moBY7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
30 This is a txt file that contains 1000 names, this will be used to create users:  <br/>
<img src="https://imgur.com/QDP9QlD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
31 This is the script that is going to be used to generate :  <br/>
<img src="https://imgur.com/Rm3PaoZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
32 The script is run and the names start generating:  <br/>
<img src="https://imgur.com/Sh8pRUR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
33 In active directory we can see that all the users have been added:  <br/>
<img src="https://imgur.com/0d5RmEu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
34 The user we created for our self has also been created:  <br/>
<img src="https://imgur.com/Bie6SBO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
35 Installation of the client (windows 10):  <br/>
<img src="https://imgur.com/9PzBVHU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
36 Successfully loaded into the client vm:  <br/>
<img src="https://imgur.com/myUeawE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
37 The IP config is all correct, as you can see it shares the same settings as the server:  <br/>
<img src="https://imgur.com/MXhOaCl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
38 Renaming this computer to CLIENT1 and making it a member of mydomain.com:  <br/>
<img src="https://imgur.com/uok0tOB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
39 Sign in with one of the accounts created to authorise that this computer is joining the domain:  <br/>
<img src="https://imgur.com/i8CqEvI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
40 This computer has successfully been added to the domain:  <br/>
<img src="https://imgur.com/YNnar7t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
41 In the server you can see under DHCP that the computer is currently leaseing an IP address:  <br/>
<img src="https://imgur.com/4lNOZkt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
42 You can also see that its a member of the domain, therefore we can use any of the accounts we created to log in to that computer:  <br/>
<img src="https://imgur.com/8nyobjB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
43 Sign in with my user account:  <br/>
<img src="https://imgur.com/Ri9MuPq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
44 Desktop of client/user computer:  <br/>
<img src="https://imgur.com/CH3LwPl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
45 Successfully logged in and part of the domain:  <br/>
<img src="https://imgur.com/jdNs2Fh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
