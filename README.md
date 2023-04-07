# Microsoft Azure Utilization & VM Environments
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (RDP)
- Virtual Networks

<h2>Operating Systems Used </h2>
- Windows 10 VM
- Linux (Ubuntu) system VM


<h2>Prerequisites</h2>
-Create two VMs (Windows 10 & Linux)
<img src="https://i.imgur.com/sFjzWkl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/dTbY6QD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

-Make sure both VMs are associated with the same Resource group and the two VMs share the same Network (Vnet)
<p>
<img src="https://i.imgur.com/uLAVkPe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/eVZDnug.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/NiM5Y9t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

In this section I will show how I checked the connectivity between the two VM environments to make sure that they can communicate back and forth. This is first ping to the from my Linux VM to the Windows VM (Using Wireshark to capture packets and see results) without the NSG blocking the ICMP connection. (ping -t)
</p>
<br />
<img src="https://i.imgur.com/bdDkQad.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<img src="https://i.imgur.com/m9ViHze.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
This ping is from my Linux VM to the Windows VM after I have configured the NSG to deny the ICMP connection. 

<img src="https://i.imgur.com/TtFxHcW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Q3ZF8kA.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p>
Lastly, for this section I made sure that I could remote SSH into my Windows VM with my user's credentials.
</p>
<br />
<p>
<img src="https://i.imgur.com/LARNhmG.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

