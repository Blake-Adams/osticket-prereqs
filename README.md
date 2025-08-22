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
<img width="305" height="168" alt="image" src="https://github.com/user-attachments/assets/0daad6f6-2705-45fd-b051-f9ecbf342d85" />


</p>
<p>
We have successfully logged into our os-Ticket vm in Active Directory. We went back out to the main screen of our Active Directory and see it is currently on and running. 
