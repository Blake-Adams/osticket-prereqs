<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://youtu.be/s2vR_i4PoBc)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create an Azure Virtual Machine Windows 10, 4 vCPUs
- Name the Virtual Machine: osticket-vm
- Create the credentials that will be used -
  Username: labuser
  Password: osTicketPassword529!
- Log into the VM with Remote Desktop

<h2>Installation Steps</h2>

<p>
<img width="1323" height="584" alt="image" src="https://github.com/user-attachments/assets/e359e6c0-134d-4a07-9396-7939e625cb52" />


</p>
<p>
  
- We'll start by creating a new virtual machine in Azure under our resource group we created for our os-Ticket vm.
- We'll then start by naming our virtual machine os-Ticket-vm and then begin to choose our specifications for the machine. 
</p>
<br />

<p>
<img width="1356" height="590" alt="image" src="https://github.com/user-attachments/assets/9e5226bf-9670-4656-b8d4-c85021cb96d0" />


</p>
<br />
  
- We'll choose Windows 10 Pro for our Operating System. We will then choose 4 vCPUs for the size of the machine that we will need for the project.
</p>
<br />
<img width="773" height="485" alt="image" src="https://github.com/user-attachments/assets/fd0b133f-84a1-47e3-ac9d-a758bb6af27b" />
</p>
<br />

- We have successfully logged into our os-Ticket vm in Active Directory.
- We downloaded the files for the osTicket onto our desktop.
- We will open the files and install the PHP Manager and Rewrite Module in order for Active Directory to run correctly.   
</p>
<br />
<img width="776" height="581" alt="image" src="https://github.com/user-attachments/assets/0bc689ea-287e-4097-9908-abee319853ff" />
</p>
<br />

- We extracted the PHP files that we installed into a new folder on our C:\ drive we named PHP. 
- We will also install Microsot Visual C++ from the installation files.
- Then we'll install MySQL as it's where we store all of the data that will be needed in the ticketing system.
- We'll run MySQL once it's finished installing. 
</p>
<br />
<img width="479" height="375" alt="image" src="https://github.com/user-attachments/assets/eb607ca5-58c1-471a-981c-1f70ee68dced" />
</p>
<br />

- We are going to open the Internet Information Systems (IIS) Program by running it as an administrator.
</p>
<br />

<img width="923" height="516" alt="image" src="https://github.com/user-attachments/assets/06481be9-ba29-4005-9842-b2c882404f38" />
</p>
<br />

- We will then register PHP Manager by running it and clicking "Register new PHP version." (PHP Manager -> C:\PHP\php-cgi.exe)

<img width="1296" height="716" alt="image" src="https://github.com/user-attachments/assets/473dd99b-2141-4c8f-8112-c174ce3771e5" />
<img width="889" height="667" alt="image" src="https://github.com/user-attachments/assets/07051cf0-faa4-4ca2-bc92-3e8f3134f5ff" />


- We will then stop and start the web server back in IIS. (We will wait about 5-10 seconds after stopping the server to start it again.)
-
- </p>
<br />
<img width="890" height="661" alt="image" src="https://github.com/user-attachments/assets/6244aaed-a564-4326-be78-f84b15074412" />


</p>
<br />

- We will upload” folder into “c:\inetpub\wwwroot. Within “c:\inetpub\wwwroot”, we will rename “upload” to “osTicket”
</p>
<br />
<img width="1185" height="671" alt="image" src="https://github.com/user-attachments/assets/02dd83bf-2f64-4c38-99e3-0b54996561a5" />
</p>
<br /> 


Click “Enable or disable an extension”
- Enable: php_imap.dll
- Enable: php_intl.dll
- Enable: php_opcache.dll
- Refresh the osTicket site in your browser, observe the changes
  
</p> 
<br />
<img width="849" height="603" alt="image" src="https://github.com/user-attachments/assets/a5f8240e-796c-4109-aed3-5977285bea83" />

</p>
<br />


Rename: ost-config.php
- From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
- To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

</p>
<br />
<img width="1113" height="585" alt="image" src="https://github.com/user-attachments/assets/ec6b22aa-b51a-403f-9e20-135cae023aad" />

</p>
<br />

Assign Permissions: ost-config.php
- Disable inheritance -> Remove All
- New Permissions -> Everyone -> All

- Continue Setting up osTicket in the browser (click Continue)
- Name Helpdesk
- Default email (receives email from customers)
- From the “osTicket-Installation-Files” folder, install HeidiSQL.
  
- Open Heidi SQL
- Create a new session, root/root
- Connect to the session
- Create a database called “osTicket”

</p>
<br />
<img width="668" height="473" alt="image" src="https://github.com/user-attachments/assets/124ee1e8-fc73-46b4-a0e4-9898e7a75c35" />
</p>
<br />

- We can log in using our admin credentials and access osTicket for the first time.
</p>
<br />
  

</p>
<br />

- Here is the dashboard of the fully installed osTicket system. It shows the activity of tickets entering the system and how they're diverted, worked, or ignored. From here, you will be able to check on the average SLA time and see if we're maintaining the proper SLA for the client or need to improve. 

</p>
<br />

<img width="1361" height="764" alt="image" src="https://github.com/user-attachments/assets/2967bd97-1424-45ab-b154-69a1a52e32a7" />

</p>
<br />
