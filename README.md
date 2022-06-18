<h1>Active Directory Home Lab</h1>


<h2>Description</h2>
Project consists of creating an Active Directory Home Lab environment through the use of Virtual Machines.  With the use of Oracle VM Virtual Box I was able to create a Windows 10 Server and a Windows 10 Client to configure Active Directory Networking.  After setting up the architechture of the network environment I used a PowerShell script to create Users to be added into the Active Directory. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Windows Service Manager</b>
- <b>Oracle VM Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Windows 10 Server</b> 

<h2>Program walk-through:</h2>

<p align="center">
Create Virtual Machine environments for both WINDOWS 10 SERVER (2019):DC and WINDOWS 10 (2019):CLIENT1<br/>
<img src="https://imgur.com/FcCwLNo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Rename Ethernet Adapters and Set Internal NIC to desired IP,Mask,Gateway,DNS:  <br/>
<img src="https://imgur.com/odaGn1E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure Local Server for Active Directory Domain Services: <br/>
<img src="https://imgur.com/rXPlLxA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure Local Server for Remote Acces and install NAT:  <br/>
<img src="https://imgur.com/WN2kGxm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure Local Server for DHCP:  <br/>
<img src="https://imgur.com/DEo4T6K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Scope for DHCP between 172.16.0.100-200:  <br/>
<img src="https://imgur.com/3SgUQeW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run PowerShell Script with while Unrestricted to add Users from .txt file:  <br/>
<img src="https://imgur.com/BL2XUHp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe created Users and DHCP Address Lease:  <br/>
<img src="https://imgur.com/xkw7NwI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm connection in CLIENT1 under created User: jbezos and check for network connectivity:  <br/>
<img src="https://imgur.com/WO1FCIL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
