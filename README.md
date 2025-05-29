<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket Installation Guide: System Requirements & Step-by-Step Setup</h1>
This guide provides a step-by-step overview of the requirements and installation process for setting up the open-source help desk ticketing system, osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Download and install osTicket files and unzip it onto your desktop
- Install internet information services (IIS) 
- Install PHP manager for IIS
- Install the rewrite module 
- Create a new folder within C:\ named "PHP"
- Unzip PHP folder into C:\PHP
- Install VC_redist.x86.exe
- Install mysql-5.5.62-win32.msi
- Activate PHP from within IIS

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/tKcyw2x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing the osTicket files, open file explorer and unzip the files into a file folder by right clicking and extracting all the necessary files to a folder and dragging the folder onto the desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/bPL6EEK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the control panel and access the windows features, once there click on internet information services -> world wide web services -> application development features -> CGI and apply the update to the windows system.
</p>
<br />

<p>
<img src="https://i.imgur.com/ACKhPBp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the osTicket-installation-file folder and download the PHP manager.
</p>
<br />

<p>
<img src="https://i.imgur.com/V51e5gQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Proceed to download the rewrite module within the folder. 
</p>
<br />

<p>
<img src="https://i.imgur.com/oAujVSh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the C:\ and create a new folder titled "PHP".
</p>
<br />

<p>
<img src="https://i.imgur.com/uVSbYcz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From inside of the osticket-installation-folder unzip the PHP folder into the C:\PHP by extracting all of the files.
</p>
<br />

<p>
<img src="https://i.imgur.com/phGClPm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install VC_redist.x86.exe from within osTicket-installation-file folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/ELR9FEY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Prior to installing mysql-5.5.62-win32.msi ensure the typical option is chosen before proceeding to install.
</p>
<br />

<p>
<img src="https://i.imgur.com/39zRu1s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Following the installation of the mysql-5.5.62-win32.msi file launch the configuration and be sure to choose standard configuration. Proceed to the username and password screen and imput "root" exactly as shown for both the username and paswword, then execute and finish the configuration.
</p>
<br />

<p>
<img src="https://i.imgur.com/zB05MeM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS and navigate to the PHP manager tab, once there register a new PHP version by going to the C:\PHP and selecting php-cgi.exe to activate it. Stop and restart the server to ensure the necessary changes were made.
</p>
<br />

<p>
<img src="https://i.imgur.com/bgPI8uL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From within the osTicket-installation-file unzip osTicket-v1.15.8 and copy the upload folder into the c:\inetpub\wwwroot and rename the upload folder to "osTicket". Following that, open IIS and proceed to stop and start the server to update the chages that were made.
</p>
<br />

<p>
<img src="https://i.imgur.com/en64Wox.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside of IIS, on the left side of the screen navigate to Sites -> Default Web Site -> osTicket. On the right side of the screen click on Browse *:80 and notice there are some features not enabled.
</p>
<br />

<p>
<img src="https://i.imgur.com/VqGZwxZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In IIS, go back to Sites -> Default Web Site -> osTicket and click on PHP manager then click enable or disable an extension. Enable php_imap.dll, php_intl.dll, and php_opcache.dll. Refresh the osTicket site in the browser and notice the changes made.
</p>
<br />

<p>
<img src="https://i.imgur.com/PTEZ7V2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside file explorer, navigate to C:\inetpub\wwwroot\osTicket\include and rename "ost-sampleconfig.php" to "ost-config.php".
</p>
<br />

<p>
<img src="https://i.imgur.com/SXeW3lP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the properties inside of ost-config.php, under security tab click advanced and disable and remove all inheritance permissions. Create a new permission and allow everyone to have full control.
</p>
<br />

<p>
<img src="https://i.imgur.com/LlpNbMs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finish setting up osTicket within the browser and when arriving at the database settings navigate back to the osTicket-installation-files and install HeidiSQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/2AIliMz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Make a connection with the database by clicking "New" and inserting "root" into both the username and password to create and connect to the session. Right click "Unnamed" and create a new database named "osTicket"
</p>
<br />
