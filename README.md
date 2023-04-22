# Configure Active Directory
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in Azure</h1>
This  outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)


<h2>Deployment and Configuration Steps</h2>

 Step 1
 
 Create two virtual machines in Azure, Windows 10(Client 1), Windows Server (DC-1)
 
 Make sure they are both created with the same Vnet and and resource group.
 
 DC-1 NIC Private IP address was placed to "static"
 
 Checked topology 
 
<p>
<img src="https://i.imgur.com/T65rap2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/lpKEDxy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2 

Ensure connectivity between the VM's

Step 3

Install Active Directory Domain Services

Step 4 

Create an admin and user in Active Directory

Step 5

Join Client to domain
</p>
<br />

<p>
<img src="https://i.imgur.com/2V3Fhpv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/BjxopsA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 6

Setup remote desktop for non admin users in Client 1
</p>
<br />

<p>
<img src="https://i.imgur.com/7GKJsWe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 7

Create many additional users

- In DC-1, open PowerShell ISE as an admin. 

- Copy script and paste into PowerShell. 

- Observe additional users being created. 

<img src="https://i.imgur.com/E66BicD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/rzgOhz4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/FkUZkYs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
