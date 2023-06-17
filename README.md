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
Now we will enable ISS with CGI. To do so, Access the Control Panel, the Program, On the upper left hand side select "Turn Windows features On or Off". Enable the IIS (Internet Information Services, expand the World Wide Web Services; Expand Application Development features; Check the CGI box and click OK to install.
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
Now we check to make sure IIS is operational by checking the loopback address of 127.0.0.1. osTicket runs off of a web browser, this will insure that osTicket will work after the instalation. 
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
Now that we know IIS is operational, we will continue with the rest of the downloads.  Atached above are the instalation files need to install osTicket.  First we will download and install PHP Manager for IIS, and download and install the Rewirte Module.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After you have completed the first set of downloads, open My Computer, go to the C: drive, and create a new file named C:PHP
</p>
<br />

<p>
<img src="https://i.imgur.com/eZW1Uys.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we have our PHP file created, we will download PHP 7.3.8.  After the download, extract the file into the PHP folder.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once the PHP file transfer is complete, download and install VC redistx86.exe and MySQL 5.5.62. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After MySQL is installed, open IIS as an administrator. This will allow is to change the php setup and enable extensions.
</p>
<br />

<p>
<img src="https://i.imgur.com/BvXR0T6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once in the IIS administrator panel, you will need to register PHP from within IIS. After registration is complete, reload IIS.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once IIS is setup (for now), we can install osTicket. After dowload is complete, Extract and copy the "upload" folder to C:\inetpub\wwwroot; within wwwroot, Rename "upload" to "osTicket"
Then open IIS admin panel and reload IIS. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to site-> Defalt -> osTicket. On the right hand side, there should be a extention "Browse *80"  Click on that. If everything has be installed correctly, a new window should come up in edge as osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once in osTicket, you can see that not all of the extentions are functional.  To enable them, go back to IIS admin panel, sites-> Default-> osTicket.  Double click PHP manager, from here you will enable a few of the extentions that are disabled. Once enabled, refresh the osTicket website and you will see that most have been activated.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are almost there! Open My Computer and go to the C drive. In C, open inetpub, then wwwroot, then osTicket. In osTicet, open Include.  Scroll down, twards the bottom will be a file named ost-samlpleconfig.php. Rename this file ost-config.php, basicly deleting the word samlple.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once in 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now you will have to assign permisssions within ostconfig.php by right clicking on the file itself, go to permissions; disable inheritance-> Remove all. Now new permissions-> Everyone all.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now ww will continue to set up osTicket. Fromhere you can use whatever kind of default email you would like to use to recieve emails from customers.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After you have set up osTicket as far as you could, we will need to download and install HeidiSQL for the database inside of osTicket. To do this, Create a new session, with root and Password. Connect with the session, create a database called "osTicket" and connect to osTickt.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue setting up osTicket with MySQL 
 -MySQL Database
 MySQL Username
 MySQL Password
 Click Install Now!
 
 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Congratulations!! hopefully it is all installed with no errors! Browse you help desk login page http://localhost/osTicket/scp/login.php
 End users osTicket url http://localhost/osTicket/ 

<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To clean up, you should delete C:inetpu\wwwroot\osTicket\setup, as well as setting the permissions to Read only on C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

