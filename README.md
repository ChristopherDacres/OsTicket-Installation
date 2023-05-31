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


- Next Download/Install <a href="https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link">PHP Manager for IIS</a>
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
 
 From the <a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files</a>, download <a href="https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link"> PHP 7.3.8 and unzip the contents into C:\PHP

  
