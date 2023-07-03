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

<h2>List of Prerequisites</h2>

- Microsoft Azure Subscription    
- Remote desktop access
- Prerequisite software 


<h2>Operating System Used </h2>
- Windows 10 (22H2)

<h2>High-Level Steps</h2>

- Step 1: Remote desktop into the VM   
- Step 2: Install / Enable IIS in Windows WITH CGI and Common HTTP Features, AND IIS Management Console
- Step 3: Download and install PHP Manager for IIS 
- Step 4: Download and install rewrite_amd64_en-US.msi   
- Step 5: Download php-7.3.8-nts-Win32-VC15-x86.zip
- step 6: Download and install VC_redist.x86.exe
- step 7: Download and install mysql-5.5.62-win32.msi
- step 8: Open IIS as an Admin, register PHP from within IIS
- step 9: Install osTicket v1.15.8
- step 10: Enable extensions
- step 11: Rename ost-config.php, then assign permissions
- step 12: Continue Setting up osTicket in the browser
- step 13: Download Heidi SQL (HeidiSQL_12.3.0.6589_Setup.exe)
- step 14: Congratulations,it's is installed
- step 15: Delete: C:\inetpub\wwwroot\osTicket\setup, set Permissions to “Read” only
 

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/AT4G7BN.png" height="65%" width="65%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/z9AU0sK.png" height="65%" width="65%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/xoVEZJl.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/TCEEEds.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/6XaU0xe.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
</p>
<p>
After connecting to the VM using RDP simply go to control panel, programs, and features and double click turn Windows features on or off. Then enable Internet Information Services (IIS), go to Application development features, and check the GCI box and common HTTP features. Then go to Internet Information Services, Web Management Tools, IIS Management Console, and check IIS management box.
</p>
<br />

<p>
<img src="https://i.imgur.com/1f0EpmS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
 <img src="https://i.imgur.com/rNZLjfI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
 <img src="https://i.imgur.com/to9Rmrr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
 <img src="https://i.imgur.com/6GggR46.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  <img src="https://i.imgur.com/MRFE7Fm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  <img src="https://i.imgur.com/Li9yNVh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now you have to download all the pre req files. Download PHPManagerForIIS_V1.5.0.msi for IIS, download rewrite_amd64_en-US.msi, first create a new directory in the C: drive called PHP then download php-7.3.8-nts-Win32-VC15-x86.zip and unzip contents into C:\PHP , and download VC_redist.x86.exe. 
 
</p>
<br />

<p>
<img src="https://i.imgur.com/CaHeyOI.png" height="65%" width="65%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/lB0zKCq.png" height="45%" width="45%" alt="Disk Sanitization Steps"/>
</p>
<p>
Due to browser limitations, you may be unable to download the php-7.3.8-nts-Win32-VC15-x86.zip file. A workaround for this would be to trust the download and press keep anyway. If that doesn't work you may have to download google chrome and download it within there. 
</p>
<br />

<p>
<img src="https://i.imgur.com/64qGzuG.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/Oq2fCx0.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/9nJC4jt.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/MI9XpG2.png" height="455%" width="55%" alt="Disk Sanitization Steps"/>
</p>
<p>
The next step is to install the MySQL-5.5.62-win32.msi file. set it to typical install, Launch Configuration Wizard (after installation) choose the standard configuration, then choose a new root password and make sure to remember it. 
</p>
<br />



<p>
<img src="https://i.imgur.com/AT4G7BN.png" height="65%" width="65%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/z9AU0sK.png" height="65%" width="65%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/xoVEZJl.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/TCEEEds.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/6XaU0xe.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
</p>
<p>
After connecting to the VM using RDP simply go to control panel, programs, and features and double click turn Windows features on or off. Then enable Internet Information Services (IIS), go to Application development features, and check the GCI box and common HTTP features. Then go to Internet Information Services, Web Management Tools, IIS Management Console, and check IIS management box.
</p>
<br />
