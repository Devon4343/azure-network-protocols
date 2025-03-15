<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />



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

1).Remote into my virtual machine and use the command prompt to ping my windows 10 virtual machine.

2).Install wireshark and filter traffic for ICMP,DHCP,DNS and observe the traffic on the command line. 

3).Configue the firewall Network Security Group that allows inbound and outbound traffic on the network.

4).Observe the traffic on command line and filter for SSH traffic.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/Z6CfIEj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First step is logging into both of virtual machines installing wireshark on windows 10 and ping the traffic from the unbuntu server 10.2.0.8 and observe the ICMP traffic.
</p>
<br />

<p>
<img src="https://i.imgur.com/jbl8SjD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure the firewall Network Securtiy Group to disable and enable inbound and outbound traffic from the unbntu server.
</p>
<br />

<p>
<img src="https://i.imgur.com/dhEOWSZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Last step I go back into wireshark and observe the inbound traffic for SSH and to do this I flitered for tcp.port == 22 and once done I type exit and enter to end the connection.
</p>
<br />
