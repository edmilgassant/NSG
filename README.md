<p align="center">
<img src="https://i.imgur.com/xr15HIN.png" alt="Microsoft Active Directory Logo"/>
</p>

In this tutorial, we are looking at traffic through wireshark using virtual machines and observing Network Security Groups within the system.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- Wireshark
- Network Protocols (SSH, DNS, ICMP,)

<h2>Operating Systems Used </h2>

- Ubuntu Server 20.04
- Windows 10 (21H2)

<h2>High-Level Steps</h2>

- Create virtual machine (Windows Server)
- Copy virtual ip address and remote connect
- Add roles on server manager
- Install Active Directory

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/HRr9zH0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installed wireshark within my virtual machine and just examing the traffic of packets.
</p>
<br />

<p>
<img src="https://i.imgur.com/hAWLj5v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
So I opened powershell command line and pinged my IP address continuisly using "ping -t 10.0.0.5" to see if there is a reply coming from that specific IP address. Timed out means that IP address is not receiving any acknowledgement from 10.0.0.5.
