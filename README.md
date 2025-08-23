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
We'll start by creating a new virtual machine in Azure under our resource group we created for our os-Ticket vm. We'll then start by naming our virtual machine os-Ticket-vm and then begin to choose our specifications for the machine. 
</p>
<br />

<p>
<img width="1356" height="590" alt="image" src="https://github.com/user-attachments/assets/9e5226bf-9670-4656-b8d4-c85021cb96d0" />


</p>
<p>
We'll choose Windows 10 Pro for our Operating System. We will then choose 4 vCPUs for the size of the machine that we will need for the project.
</p>
<br />
<img width="773" height="485" alt="image" src="https://github.com/user-attachments/assets/fd0b133f-84a1-47e3-ac9d-a758bb6af27b" />
</p>
<br />
We have successfully logged into our os-Ticket vm in Active Directory. We downloaded the files for the osTicket onto our desktop. We will open the files and install the PHP Manager and Rewrite Module in order for Active Directory to run correctly.   
</p>
<br />
<img width="776" height="581" alt="image" src="https://github.com/user-attachments/assets/0bc689ea-287e-4097-9908-abee319853ff" />
</p>
<br />
We extracted the PHP files that we installed into a new folder on our C:\ drive we named PHP. We will also install Microsot Visual C++ from the installation files. Then we'll install MySQL as it's where we store all of the data that will be needed in the ticketing system. We'll run MySQL once it's finished installing. 
</p>
<br />
<img width="479" height="375" alt="image" src="https://github.com/user-attachments/assets/eb607ca5-58c1-471a-981c-1f70ee68dced" />
</p>
<br />
-We are going to open the Internet Information Systems (IIS) Program by running it as an administrator. We will then register PHP Manager by running it and clicking "Register new PHP version." We will then stop and start the web server. 
</p>
<br />
<img width="923" height="516" alt="image" src="https://github.com/user-attachments/assets/06481be9-ba29-4005-9842-b2c882404f38" />

</p>
<br />
-We will then upload” folder into “c:\inetpub\wwwroot. Within “c:\inetpub\wwwroot”, we will rename “upload” to “osTicket”
</p>
<br />
<img width="1185" height="671" alt="image" src="https://github.com/user-attachments/assets/02dd83bf-2f64-4c38-99e3-0b54996561a5" />
</p>
<br />

</p>
<br />

</p>
<br />

</p>
<br />

</p>
<br />

</p>
<br />
