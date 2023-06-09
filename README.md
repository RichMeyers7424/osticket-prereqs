<p align="center">
<img src="https://i.imgur.com/uT7SVV8.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket. I will be using Azure to create a Virtual Machine to install osTicket. This step is not nessessary to install or use osTicket.
<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisits </h2>

- Azure Virtual Machine
- [osTicket Installation files](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) 
- Heidi SQL

<h2>Installation Steps</h2>

- Step 1: Azure virtual machine deployment
- Step 2: Remote Access to VM
- Step 3: Install PHP
- Step 4: Install Rewrite Module
- Step 5: Create PHP
- Step 6: Install C++
- Step 7: Install Heidi SQL
- Step 8: Install osTicket
 
</p>
<br />

<h2>Step 1</h2>

</p>
<br />

<p>
First, we will create a virtual machine in azure to set up and run osTicket.
 
 </p>
<br />

<img src="https://i.imgur.com/lCxkFRI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
Once we have our Virtual Machine created, we will remote access the vm using Remote desktop conection. To do so we must obtain the ip address of our vm. You can find it in the vm's files.
</p>
<br />

<p>
<img src="https://i.imgur.com/J4lEPsw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

<p>
If your on Windows, you can use the search bar to access Remot Desktop Connection. If your using a Mac, you'll have to download windows remote desktop in the app store.
</p>
<br />

<p>
<img src=https://i.imgur.com/O8kKB3g.png"" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

 <p>
Now that we have established connection with the vm, we will have to set up a few things before we are able to install osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/R6kKxyr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

 <p>
Now we will enable ISS with CGI. To do so, 1-Access the Control Panel > 2-Program > 3-On the upper left hand side select "Turn Windows features On or Off"> 4- Enable the IIS (Internet Information Services) > 5-Expand the World Wide Web Services > 6-Expand Application Development features > 7-Check the CGI box and click OK to install.
 </p>
<p>
<br />
 
<p>
<img src="https://i.imgur.com/qCJdSqx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<p>
<br />  

 <p>
Now we check to make sure IIS is operational by checking the loopback address of 127.0.0.1
<br />
 </p>
<p>
<br /> 
 
<p>
<img src="https://i.imgur.com/GQgjd72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
