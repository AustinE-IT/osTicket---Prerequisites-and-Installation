<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


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

