<p align="center">
<img src="https://i.imgur.com/uT7SVV8.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>List of Prerequisits </h2>

- Azure Virtual Machine
- [osTicket Installation files](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) 
- Heidi SQL

<h2>Installation Steps</h2>
 In this tutorial, you will find all the materials needed with an in depth explination of osTicket, how to install, troubleshoot and teach others how to use and install osTicket!
</p>
<br />


<p>
<img src="https://i.imgur.com/lCxkFRI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, we will create a virtual machine in azure to set up and run osTicket. 
</p>
<br />

<p>
<img src="https://i.imgur.com/qCJdSqx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we will enable ISS with CGI. To do so, 1-Access the Control Panel > 2-Program > 3-On the upper left hand side select "Turn Windows features On or Off"> 4- Enable the IIS (Internet Information Services) > 5-Expand the World Wide Web Services > 6-Expand Application Development features > 7-Check the CGI box and click OK to install.


<br />     https://i.imgur.com/GfBiWsU.png

<p>
<img src="https://i.imgur.com/GQgjd72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we check to make sure IIS is operational by checking the loopback address of 127.0.0.1
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
