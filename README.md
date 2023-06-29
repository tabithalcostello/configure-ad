<p align="center"> 
<img src="https://i.imgur.com/gW9mWz0.png"  height="50%" width="50%" alt="Microsoft Active Directory" /></a>  

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

<h2>Rename</h2>

<p> 
<img src="https://i.imgur.com/qTktgXH.png" height="80%" width="80%" alt="Create a Domain Controller"/>
</p>
<p>
In Microsoft Azure, create a Virtual Machine (VM) that will be used as a Domain Controller (DC). For this instance, Windows Server 22 Data Center was selected. Select an appropriate VM size (Standard 2vpcu and 16 Gib Memory). Create and record username and password. Once created in Azure, open DC-1's "Networking," and set the ipconfiguration to Static. 
</p>
<br />

<p> 
<img src="https://i.imgur.com/0bnhEYP.png" height="80%" width="80%" alt="Create a Client"/>
</p>
<p>
In Microsoft Azure, create a second VM, which will act as the Client. We connected the same Resource Group used by DC-1. Select Windows 10 Pro. Create and record username and password. Check the license agreement box in the corner. In the Network section, select the same network used by DC-1 (DC-1-vnet).
</p>
<br />

<p> 
<img src="https://i.imgur.com/iBPMiat.png" height="80%" width="80%" alt="Connect to Remote Desktop"/>
</p>
<p>
In Microsoft Azure, collect the DC-1's and Client's ip address. In Microsoft Remote Desktop, add PC with the respective IP Address, then connect. Check connectivity between the two VMs. In the Client VM, pertual ping DC's ip address. 
</p>
<br />

<p>
<img src="https://i.imgur.com/O3pPOou.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the DC-1 VM, access wf.msc to change the Firewall settings. In the Inbound Rules, scroll to Protocol. Check that ICMPv4 are Enabled. Refresh the Windows Defender Wall. Afterward, return to Client VM and check the connectivity dispalyed in the perpetual ping.
</p>
<br />
<br />

<p> 
<img src="https://i.imgur.com/QZ6Nsjw.png" height="80%" width="80%" alt="Install AD"/>
</p>
<p>
In DC-1, access the Server Manager, select "Add Roles and Features." In the section "Server Roles," check the box for "Active Directory Domain Services." Check Add. Click Install. 
</p>
<br />

<p>
<img src="https://i.imgur.com/LkQvtEa.png" height="80%" width="80%" alt="AddRoles"/>
</p>
<p>
Once the initial installation is complete, a yellow triangle will appear by the flag. Click on it. Click on "Promote this server to a domain controller."
</p>
<br />

<p>
<img src="https://i.imgur.com/mwnT8Xb.png" height="80%" width="80%" alt="AddRoles"/>
</p>
<p>
In the Deployment Configuration, check "Add a a new forest." In the empty box next to Root domain name, insert the name of your domain controller. In this case, mydomain.com. Click Next. Insert password when prompted. Click until "Install" is an option, and click on it. The computer will Restart upon complete installation.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Log into your DC with your domain name with user name. [Ex. mydomain.com\labuser]
</p>
<br />

<p>
<img src= height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
