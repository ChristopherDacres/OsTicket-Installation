<p align="center">
<img src="https://i.imgur.com/mL4d1tt.jpg"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
In this tutorial we will be going through the full installation for osTicket and the prerequisites required to meet installation. We will install osTicket on an Microsoft Azure VM (Virtual Machine). We will need to have a Virtual Machine setup and accessed using Remote Desktop. Refer to this link <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6"</a>Installation Files

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- Internet Information Services (IIS)
- MySQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Dowloading Installation Files </h2>

- Copy and Paste the URL into Microsoft Edge on the Virtual Machine (Please note this is to be download in the Virtual Machine)

<img src="https://i.imgur.com/GrH9Yg5.png"/>

<h2>Install/Enable IIS in Windows WITH CGI and Common HTTP Features</h2>

- Go to Control Panel
- Programs 
- Turn Windows Features On or OFF
- Click and Expand Internet Information Services
- Click and expand Web Managment Tools
- Check IIS Managment Console
- Click and expand World Wide Web Services
- Click and expand Application Development Features
- Check CGI
- Select OK
- Select Close

<img src="https://i.imgur.com/M4F1qyF.png"/>
<img src="https://i.imgur.com/D0DWhVX.png"/>
<img src="https://i.imgur.com/GoKJ7va.png"/>
<img src="https://i.imgur.com/s736uW3.png"/>
<img src="https://i.imgur.com/IbsqWbu.png"/>


Download/Install <a href="https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link">PHP Manager for IIS</a>
from <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a>

 <img src="https://i.imgur.com/i2O5lya.png"/>
  
  <b> Next Download/Install <a href="https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link"> Rewrite Module</a> from <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a>
  
  <img src="https://i.imgur.com/tQw3mny.png"/>
 
 <h2>Create the directory C:\PHP</h2>
 
 - Open File Explorer
 - This PC
 - Windows (C:) Drive
 - Right Click to add NEW FOLDER
 - Name it "PHP"
  
 <img src="https://i.imgur.com/tV5tJIa.png"/>
 <img src="https://i.imgur.com/kwU3xAt.png"/>
 
 <h2>Next From the <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a>, Download/Install <a href="https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link"> PHP 7.3.8</a> and unzip the contents into C:\PHP </h2>
 
 - Right Click to EXTRACT ALL
 - Click Browse
 - This PC
 - Windows (C:)
 - Click PHP
 - Select EXTRACT
 
 <img src="https://i.imgur.com/HIH8uce.png"/>
 <img src="https://i.imgur.com/M2f9mZa.png"/>
 <img src="https://i.imgur.com/Mq8nOkb.png"/>
 
 Next From the <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a> Download/Install <a href="https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link"> VC_redist.x86.exe
 
 <img src="https://i.imgur.com/uS4vYKn.png"/>
 
   <h2>Next From the <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a> Download/Install <a href="https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link"> MySQL 5.5.62 </h2>
    
- Typical Setup
- Launch Configuration Wizard (after install)
- Standard Configuration
- Username: ROOT
- Password: Password1
    
    <img src="https://i.imgur.com/bXAKRqe.png"/>
    <img src="https://i.imgur.com/01bmt4W.png"/>
    <img src="https://i.imgur.com/FCA7a8q.png"/>
    <img src="https://i.imgur.com/qOtqyCW.png"/>
    <img src="https://i.imgur.com/pUul3IO.png"/>
    <img src="https://i.imgur.com/rvVZ5aU.png"/>
    <img src="https://i.imgur.com/Ut3NkFE.png"/>
    
    <h2>Open IIS as an Admin</h2>
    
    - Type IIS in start menu
    - Click on Run as Adminstrator
    - Select PHP Manager
    - Select Register new PHP Version
    - Click Browse
    - Select PHP CGI (make sure PHP executable)
    - Select OK
    - Click Restart 
    
    <img src="https://i.imgur.com/Zg3cfkQ.png"/>
    <img src="https://i.imgur.com/q7mADKh.png"/>
    <img src="https://i.imgur.com/DJu6bOZ.png"/>
    <img src="https://i.imgur.com/2oY1hkZ.png"/>
    <img src="https://i.imgur.com/jh1lkQi.png"/>
    <img src="https://i.imgur.com/9PFiixZ.png"/>
    
    <h2>Next From the <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a>, Download/Install <a href="https://drive.google.com/file/d/1VeVXKlzHDRjeaVUL99ptq7qYbrbXdFxJ/view?usp=drive_link">osTicket</a>

- Extract and copy “upload” folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
     
     <img src="https://i.imgur.com/R1ey3p7.png"/>
     <img src="https://i.imgur.com/4zednt0.png"/>
     
     <h2>Reload IIS (Open IIS, Stop and Start the server)</h2>
     
- Go to Sites
- Default
- osTicket
- On the right, click “Browse *:80”

     
     <img src="https://i.imgur.com/M8tRnEI.png"/>
     
     <h2> Note that some extensions are not Enabled </h2>
     
- Go back to IIS, sites -> Default -> osTicket
- Double-click PHP Manager
- Click “Enable or disable an extension”
- Enable: php_imap.dll
- Enable: php_intl.dll
- Enable: php_opcache.dll
- Refresh the osTicket site in your browse, observe the changes

     <img src="https://i.imgur.com/CNiCtVy.png"/>
     <img src="https://i.imgur.com/vRKpqtT.png"/>

      
    
    


 
 
 
 
 

  
