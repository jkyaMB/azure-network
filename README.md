<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create some smaple fils shares with various permissions 
- Then attempting to access files shares as a normal user 
- Create an Accountants security group, assigning permissions and test access 
  

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We'll start this project by logining into our domain admin account and our Client- 1 Virtual machines. Creating 4 different folders and set permisson for each, skipping one for now. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In our Client-1 we will navigate the share folder and run DC-1, seeing which folder we can access and one we are restricted from. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lastley, we will create a security group called Accountants ans assign permisson and test its access. Logining out of client-1 and into DC-1, we'll assgin some user to the accountants security group and log back in as one of the users. Sigining in as one user and testing which access we had assign to it earlier. 
</p>
<br />
