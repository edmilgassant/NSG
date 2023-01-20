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

- Create virtual machines (Windows Server and Ubuntu)
- Installed wireshark
- Capture traffic and view only in ICMP
- Use powershell to view responses of packets from Windows10VM to LinuxVM

<h2>Examination and Action Steps</h2>

<p>
<img src="https://i.imgur.com/f8NYYbr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created two VMs. One on Windows 10 and the other on Linux. Going to remote connect into Windows 10 VM and install wireshark. Going to inspect traffic while interacting with LinuxVM. Lets capture packets!
</p>
<br />

<p>
<img src="https://i.imgur.com/yWdHpdG.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Just capturing packets. It is basically just showing random packets moving around on Windows10VM. Now I'll use icmp in the small search engine and inspect traffic on LinuxVM 


<p>
<img src="https://i.imgur.com/E8kJmD5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After searching icmp. I copied LinuxVM private address and opened powershell to ping LinuxVM private IP adress and started recieving traffic from LinuxVM while on Windows10VM. Pretty cool!
