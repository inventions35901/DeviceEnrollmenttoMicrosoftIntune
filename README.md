# Device Enrollment to Microsoft Intune
Hands-on lab demonstrating Windows device enrollment into Microsoft Intune using Microsoft Entra ID, including MFA setup, Windows Hello configuration, and compliance verification.
<h1>Active Directory Home Lab</h1>

<h2>Description</h2>

This project showcases the design and deployment of a fully functional Active Directory home lab using Oracle VirtualBox, simulating a real-world enterprise network environment.

In this lab, I implemented and configured key infrastructure services including Active Directory Domain Services (AD DS), DNS, DHCP, and NAT-based routing. I also managed domain users, group policies, and network configurations to replicate common system administration tasks.

This project highlights hands-on experience with Windows Server environments, network infrastructure, and troubleshooting—demonstrating practical skills applicable to entry-level IT and system administration roles.

<br />

<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b>
- <b>Active Directory Domain Services</b>
- <b>DHCP Server</b>
- <b>DNS Server</b>
- <b>Routing and Remote Access (RRAS)</b>
- <b>Oracle VirtualBox</b>

<br />

<h2>Environments Used</h2>

- <b>Windows Server 2019</b>
- <b>Windows 10</b>
- <b>Oracle VirtualBox</b>

<br />

<h2>Network Architecture</h2>

<p align="center">
<img src="00-network-diagram.png" width="80%">
</p>

<br />

<h2>Program Walk-through:</h2>

<p align="center">

Create Domain Controller Virtual Machine<br/>
<i>Provision a Windows Server virtual machine to act as the domain controller.</i><br/>

<img src="01-create-dc-vm-1.png" width="80%"/>
<br/>
<img src="01-create-dc-vm-2.png" width="80%"/>

<br/><br/>

Install Windows Server 2019<br/>
<i>Install the Windows Server operating system on the domain controller VM.</i><br/>

<img src="02-install-windows-server-1.png" width="80%"/>
<br/>
<img src="02-install-windows-server-2.png" width="80%"/>

<br/><br/>

Configure Static IP Address<br/>
<i>Assign a static IP address to ensure consistent network communication.</i><br/>

<img src="03-configure-static-ip.png" width="80%"/>

<br/><br/>

Install Active Directory Domain Services<br/>
<i>Add the Active Directory Domain Services role to the server.</i><br/>

<img src="04-install-ad-ds-1.png" width="80%"/>
<br/>
<img src="04-install-ad-ds-2.png" width="80%"/>

<br/><br/>

Create Active Directory Domain<br/>
<i>Promote the server to a domain controller and create a new domain.</i><br/>

<img src="05-create-domain-1.png" width="80%"/>
<br/>
<img src="05-create-domain-2.png" width="80%"/>

<br/><br/>

Configure NAT using Routing and Remote Access<br/>
<i>Enable NAT using RRAS to allow internal network access to external resources.</i><br/>

<img src="06-configure-nat-rras-1.png" width="80%"/>
<br/>
<img src="06-configure-nat-rras-2.png" width="80%"/>
<br/>
<img src="06-configure-nat-rras-3.png" width="80%"/>

<br/><br/>

Configure DHCP Scope<br/>
<i>Set up DHCP to automatically assign IP addresses to client machines.</i><br/>

<img src="07-configure-dhcp-scope.png" width="80%"/>
<br /><br />

Create Domain Admin Account<br/>
<i>Create a domain administrator account for managing the environment.</i><br/>

<img src="08-create-domain-admin-1.png" width="80%"/>
<br/>
<img src="08-create-domain-admin-2.png" width="80%"/>
<br/>
<img src="08-create-domain-admin-3.png" width="80%"/>

<br/><br/>

Create Windows 10 Client Virtual Machine<br/>
<i>Provision a client machine to join and interact with the domain.</i><br/>

<img src="09-create-windows-10-client-vm-1.png" width="80%"/>
<br/>
<img src="09-create-windows-10-client-vm-2.png" width="80%"/>
<br/>
<img src="09-create-windows-10-client-vm-3.png" width="80%"/>

<br/><br/>

Verify Network Connectivity<br/>
<i>Ensure the client machine can communicate with the domain controller and network.</i><br/>

<img src="10-verify-network-connectivity-1.png" width="80%"/>
<br/>
<img src="10-verify-network-connectivity-2.png" width="80%"/>
<br/>
<img src="10-verify-network-connectivity-3.png" width="80%"/>

<br/><br/>

Join Windows 10 Client to Domain<br/>
<i>Connect the client machine to the Active Directory domain.</i><br/>

<img src="11-join-client-to-domain-1.png" width="80%"/>
<br/>
<img src="11-join-client-to-domain-2.png" width="80%"/>

<br /><br />

Verify Computer Appears in Active Directory<br/>
<i>Confirm the client machine is successfully added to the domain.</i><br/>

<img src="12-verify-computer-in-ad.png" width="80%"/>
<br /><br />

Run PowerShell Script to Generate Users<br/>
<i>Automate user account creation using a PowerShell script.</i><br/>

<img src="13-run-powershell-user-script-1.png" width="80%"/>
<br/>
<img src="13-run-powershell-user-script-2.png" width="80%"/>
<br/>
<img src="13-run-powershell-user-script-3.png" width="80%"/>

<br/><br/>

</p>

<h2>Skills Demonstrated</h2>

• Active Directory Deployment  
• DNS and DHCP Configuration  
• NAT and Routing  
• Domain User Management  
• PowerShell Automation  
• Virtualized Enterprise Network Setup  

<br />

<h2>Project Outcome</h2>

This lab successfully demonstrates how a corporate Windows domain environment is built and managed. The project simulates real-world enterprise infrastructure where domain users authenticate to centralized services through a Domain Controller.
