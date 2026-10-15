<h1>Active Directory Lab</h1>


<h2>Description</h2>
In this lab, we walk through the process of creating an Active Directory environment using two virtual machines in Oracle Virtual Box. We will create one VM as the domain controller with the following installed and configured: AD, RAS/NAT, DHCP, and DNS. The second virtual machine will serve as the internal network that will join to the domain. 
<br />


<h2>Languages and Utilities Used</h2>
 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
Change adaptor options and determine which Ethernet port is connected to the Internet, and which is internal. Rename accordingly:<br/>
<img src="https://imgur.com/Qph3VKh.png" height="80%" width="80%" alt=/>
<br />
<br />
<br/>
<img src="https://imgur.com/KPuyH8n.png" height="80%" width="80%" alt=/>
<br />
<br />
Configure IP for internal network. DC serves as gateway, and AD will provide DNS,configure as own IP or use loopback address: <br/>
<img src="https://imgur.com/IYatyc8.png" height="80%" width="80%" alt=/>
<br />
<br />
Rename PC as a domain controller:  <br/>
<img src="https://imgur.com/pL6f21g.png" height="80%" width="80%" alt=/>
<br />
<br />
Install Active Directory Domain Services:  <br/>
<img src="https://imgur.com/D6hFACr.png" height="80%" width="80%" alt=/>
<br />
<br />
Promote server to a domain controller :  <br/>
<img src="https://imgur.com/kOT6dOp.png" height="80%" width="80%" alt=/>
<br />
<br />
Create an organizational unit to add a dedicated domain admin account:  <br/>
<img src="https://imgur.com/YDXL1fI.png" height="80%" width="80%" alt=/>
<br />
<br />
Create account and promote it to an admin. Sign out and sign into new admin account: <br/>
 <img src="https://imgur.com/DzSS8XF.png" height="80%" width="80%" alt=/>
<br />
<br />
Install Remote Access and configure Network Address Translation to the INTERNET network: <br/>
<img src="https://imgur.com/BL0G20C.png" height="80%" width="80%" alt=/>
<br />
<br />
<img src="https://imgur.com/2Wj1HON.png" height="80%" width="80%" alt=/>
<br />
<br />
Install DHCP to allow clients to receive an IP address automatically:
<img src="https://imgur.com/Q8BxY9z.png" height="80%" width="80%" alt=/>
<br />
<br />
Go into DHCP to configure the scope and set IP of DC as default gateway :
<img src="https://imgur.com/rDvFsbm.png" height="80%" width="80%" alt=/>
<br />
<br />
<img src="https://imgur.com/ZTLx1DA.png" height="80%" width="80%" alt=/>
<br />
<br />
Create second VM, change network adapter settings to Internal Network, and install Windows 10 ISO:
<img src="https://imgur.com/mCTId00.png" height="80%" width="80%" alt=/>
<br />
<br />
<img src="https://imgur.com/j82UVni.png" height="80%" width="80%" alt=/>
<br />
<br />
Open command line to run ipconfig to confirm and ping a website to confirm internet connection to DC:
<img src="https://imgur.com/icyr0sD.png" height="80%" width="80%" alt=/>
<br />
<br />
Lastly, rename the PC and join the domain:
<img src="https://imgur.com/N7ucZ87.png" height="80%" width="80%" alt=/>
 
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
