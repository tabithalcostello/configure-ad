<p align="center"> 
<img src="https://i.imgur.com/awz0ZA7.png" height="50%" width="50%" alt="Microsoft Active Directory"/>
</p>

<h1>Configure Active Directory</h1>
This tutorial outlines how to install Active Directory (AD) and configure AD.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems </h2>

- Windows 10
- Windows Server 22 Data Center</b> 

<h2> Process </h2>

- Create two Virtual Machines (Domain Controller and Client)
- Configure in Server Manager the Active Directory
- 

<h2>Rename</h2>

<p> 
<img src="https://i.imgur.com/qTktgXH.png" height="80%" width="80%" alt="Create a Domain Controller"/>
</p>
<p>
In Microsoft Azure, create a Virtual Machine (VM). The first VM will be set up to be the Domain Controller (DC). Add a Resource Group Name (AD-Lab). Add a VM name (DC-1). Select Windows Server 22 Data Center. Select an appropriate VM size (Standard 2vpcu and 16 Gib Memory). Create and record username and password. 
</p>
<br />

<p> 
<img src="https://i.imgur.com/0bnhEYP.png" height="80%" width="80%" alt="Create a Client"/>
</p>
<p>
In Microsoft Azure, create a VM, which will act as the Client. Be sure to select the same Resource Group used by DC-1. Select Windows 10 Pro. Create and record username and password. Check the license agreement box in the corner. In the Network section, select the same network used by DC-1 (DC-1-vnet).
</p>
<br />

<p> 
<img src="https://i.imgur.com/iBPMiat.png" height="80%" width="80%" alt="Connect to Remote Desktop"/>
</p>
<p>
In Microsoft Azure, collect the DC-1's and Client's IP address. In Microsoft Remote Desktop, add PC with the respective IP Address, then connect. 
</p>
<br />

<p> 
<img src="https://i.imgur.com/RYleh3z.pn" height="80%" width="80%" alt="Install AD"/>
</p>
<p>
In the Server Manager, select "Add Roles and Features." In the section "Server Roles," check the box for "Active Directory Domain Services." Check Add. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
<br />
