<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create a Windows 10 Virtual machine and Create a Linux 'Ubuntu' virtual machine)
- Use Remote Desktop to connect to your Windows 10 Virtual Machine and install Wireshark
- Open Wireshark and filter for ICMP traffic only
- Retrieve the private IP address of the Ubuntu VM and attempt to ping it from within the Windows 10 VM
- From The Windows 10 VM, open and attempt to ping a public website (such as www.google.com) from command line or PowerShell and observe the traffic in WireShark
- From Wireshark, Observe the DHCP traffic(ipconfig /renew), Observe the SSH traffic (username, pwd, etc), Observe the SSH traffic (nslookup) and Observe RDP traffic only (tcp.port == 3389)

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/PaanT8z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<p>
Virtual machine of windows and linux(Ubuntu) created in Microsoft Azure 
</p>
<br />

<p>
<img src="https://i.imgur.com/oueelAM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing ICMP om Wireshark and Powershell commands
</p>
<br />

<p>
<img src="https://i.imgur.com/cGMuBnM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing the UDP port=67 - UDP port=68 (DHCP) on Wiresharks and Powershell commands
</p>
<br />
