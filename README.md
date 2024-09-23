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

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- Virtual Machine
- Internet Information Services (IIS) Web Server
- mySQL Database
- osTickets files and downloads


<h2>Installation Steps</h2>

<p>
<img width="596" alt="image" src="https://github.com/user-attachments/assets/7f9f049b-f8d0-4a86-b000-d356959b5cf0">
</p>
<p>
Create a VM in Microsoft Azure (Mine is called osTicket-vm)
</p>
<br />
<br />
<br />
<p>
<img width="860" alt="image" src="https://github.com/user-attachments/assets/0b116553-a419-4f12-893e-5d94d5f7f414">
</p>
<p>
Enable IIS in windows with CGI 
<br />
<br />
<br />
<p>
<img width="845" alt="image" src="https://github.com/user-attachments/assets/00584ce4-7e2c-40a0-9924-c23710a149b6">
</p>
<p>
Install osTicket installation files: PHP Manager for IIS and rewrite module 
</p>
<br />
<br />
<br />

<p>
<img width="856" alt="image" src="https://github.com/user-attachments/assets/262e6106-6462-4d4f-8398-b7154e93fe00">
</p>
<p>
Create PHP Directory to unzip php installation zip file
</p>

<br />
<br />
<br />
<p>
<img width="857" alt="image" src="https://github.com/user-attachments/assets/74ba5a56-680b-4675-ad0c-ee2432b06f69">
</p>
<p>
Install osTicket installation files: VC_Redist.x86.exe and mySQL for the database with standard configuration
</p>
<br/>
<br />
<br />

<p>
<img width="857" alt="image" src="https://github.com/user-attachments/assets/74ba5a56-680b-4675-ad0c-ee2432b06f69">
</p>
<p>
Install osTicket installation files: VC_Redist.x86.exe and mySQL for the database with standard configuration
</p>
<br/>
<br />
<br />

<p>
<img width="853" alt="image" src="https://github.com/user-attachments/assets/cf4a7362-ee78-4e8b-9f5d-7762691593a8">
</p>
<p>
Open IIS as an administrator, then register PHP executable
</p>
<br/>
<br />
<br />

<p>
<img width="855" alt="image" src="https://github.com/user-attachments/assets/39a1d3f6-0001-44db-8256-f52b45996303">
</p>
<p>
Reload IIS (Stop and Start the server). From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”.
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”
 
</p>
<br/>
<br />
<br />

<p>
<img width="856" alt="image" src="https://github.com/user-attachments/assets/3a7dfc62-b4b5-41d5-b595-61d3fdd21862">
</p>
<p>
Open IIS as an admnistrator and reload it (Stop and Start the server). Go to sites -> Default -> osTicket. Double click PHP Manager, click "enable or disable an extension" and make sure the following are enabled: php_imap.dll, php_intl.dll, php_opcache.dll
</p>
<br/>
<br />
<br />

<p>
<img width="854" alt="image" src="https://github.com/user-attachments/assets/f1c370a2-8ec7-4f11-af68-cf98fcd817aa">
</p>
<p>
In IIS go to sites -> Default -> osTicket. on the right, click "Browse *.80" to verify osTicket is connected and verify the previous extensions have been enabled
</p>
<br/>
<br />
<br />

<p>
<img width="856" alt="image" src="https://github.com/user-attachments/assets/b1cfc23e-6df3-4f0e-94ea-4001feed162b">
</p>
<p>
Fill out the following information.
</p>
<br/>
<br />
<br />

<p>
<img width="853" alt="image" src="https://github.com/user-attachments/assets/38027b4d-0cb6-4de5-a833-b293955195cd">
</p>
<p>
Install HeidieSQL from the osTicket installation folder
</p>
<br/>
<br />
<br />
Open Heidi SQL
Create a new session, root/root
Connect to the session
Create a database called “osTicket”

<p>
<img width="857" alt="image" src="https://github.com/user-attachments/assets/00d2ba9b-3005-4daf-b4a7-37335aeb1e0e">
</p>
<p>
Open Heidi SQL, Create a new session: root/root, Connect to the session, Create a database called “osTicket”
</p>
<br/>
<br />
<br />

<p>
<img width="855" alt="image" src="https://github.com/user-attachments/assets/7b680f44-5fbb-4118-be90-45232b47a6e4">
</p>
<p>
fillout database section then click install now
</p>
<br/>
<br />
<br />


<p>
<img width="856" alt="image" src="https://github.com/user-attachments/assets/3e41ffc7-d61d-4f97-a2ac-e30498832d3f">
</p>
<p>
Successful installation will be greeted with Congratulations page
</p>
<br/>
<br />
<br />
