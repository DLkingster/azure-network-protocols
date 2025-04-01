<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create Windows 10 Virtual Machine (VM).
- Create Virtual Network (VNET) and Subnet.
- Use Remote Desktop to connect to your Windows 10 Virtual Machine
- Configuring a Firewall [Network Security Group]
- Wireshark packet capture, open Powershell command line, observe ping request, observe website traffic.

<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/user-attachments/assets/92dabbf1-2399-43ad-bba7-b8420165897a"/>
</p>
<p>
Enter virtual machines in the search. Under Services, select Virtual machines. In the Virtual machines page, select Create and then Azure virtual machine. The Create a virtual machine page opens.Under Instance details, enter myVM for the Virtual machine name and choose Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2 for the Image. Leave the other defaults.Under Administrator account, provide a username, such as azureuser and a password. Under Inbound port rules, choose Allow selected ports and then select RDP (3389) and HTTP (80) from the drop-down. Leave the remaining defaults and then select the Review + create button at the bottom of the page. After validation runs, select the Create button at the bottom of the page.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/ca3068d9-aab3-4040-88ed-128120ebef27"/>
</p>
<p>
On the overview page for your virtual machine, select the Connect > RDP. In the Connect with RDP tab, keep the default options to connect by IP address, over port 3389, and click Download RDP file. Open the downloaded RDP file and click Connect when prompted. In the Windows Security window, select More choices and then Use a different account. Type the username as localhost\username, enter the password you created for the virtual machine, and then click OK. You may receive a certificate warning during the sign-in process. Click Yes or Continue to create the connection. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f9ead750-eeb5-42b3-9c03-f73ce591581a"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
