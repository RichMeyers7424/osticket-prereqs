<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

System Requirements:

Web server (e.g., Apache, Nginx)
PHP version 7.4 or later
MySQL or MariaDB database server
Download osTicket:

Visit the official osTicket website at https://osticket.com/ and navigate to the "Download" section.
Choose the latest stable release and download the ZIP package to your PC.
Extract Files:

Extract the downloaded ZIP package to a location on your PC. This will create a directory containing osTicket files.
Configure Web Server:

Set up a virtual host or configure your web server to point to the directory where you extracted osTicket files.
Create a Database:

Access your MySQL or MariaDB server and create a new database for osTicket.
Create a user with appropriate privileges and assign it to the newly created database.
Configure osTicket:

Rename the "include/ost-sampleconfig.php" file to "include/ost-config.php".
Open "include/ost-config.php" using a text editor and provide the necessary database connection details (database name, username, password).
Install osTicket:

Open a web browser and access the URL where you configured osTicket (e.g., http://localhost/osticket).
The installation wizard should start automatically.
Follow the on-screen instructions, providing information such as the database connection details, administrative email, and system settings.
Once the installation is complete, the wizard will prompt you to create an administrative account.
Finalize Installation:

After creating the administrative account, the installation process should be complete.
Log in to the osTicket administrative interface and configure additional settings as needed.



<h2>Installation Steps</h2>

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
Now we will enable ISS with CGI.
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
