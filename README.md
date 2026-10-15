<h1>Active Directory Lab</h1>


<h2>Description</h2>
In this lab, we walk through the process of creating an Active Directory environment using two virtual machines in Oracle Virtual Box. We will create one VM as the domain controller with the following installed and configured: AD, RAS/NAT, and DHCP Scope. The second virtual machine will serve as the internal network.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
Change adaptor options and determine which Ethernet port is connected to the Internet, and which is internal. Rename accordingly:<br/>
<img src="https://imgur.com/Qph3VKh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>
<img src="https://imgur.com/KPuyH8n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure IP for internal network. DC serves as gateway, and AD will provide DNS,configure as own IP or use loopback address: <br/>
<img src="https://imgur.com/IYatyc8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Rename PC as a domain controller:  <br/>
<img src="https://imgur.com/pL6f21g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Active Directory Domain Services:  <br/>
<img src="https://imgur.com/D6hFACr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Promote server to a domain controller :  <br/>
<img src="https://imgur.com/kOT6dOp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
