<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create Resources in Azure
- Install Active Directory
- Create an Admin and User Account in Active Directory 
- Create Security Groups
- Create Share Files
- Set Share File Permissions

<h2>Deployment and Configuration Steps</h2>

<p>

![1 Install Active Directory](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/2d76ec36-86df-4d4b-bfcb-353ffec3fc44)

</p>
<p>
After creating your resources in Microsoft Azure, log in to your domain controller virtual machine and begin installing Active Directory Domain Services. 
</p>
<br />

<p>

![2 add new forest](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/c2d7fcf7-6cbc-4d1d-9818-e5a8a5e497a2)

</p>
<p>
Begin configuring Active Directory Domain Services by adding a new forest. This will be your root domain name. Finish the installation and restart your virtual machine. 
</p>
<br />

<p>

![3 employee OU](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/bcdb5e79-81a9-4dec-8672-dc9d5d2f4afa)

</p>
<p>
From the Active Directory, you can create new Organizational Units. In this case, you will create an Employee Organizational Unit for access to normal users. 
</p>
<br />

<p>

![4 ADMINS OU](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/d830c7e1-e699-46c8-a3b8-e0e88f32948b)

</p>
<p>
You will then create an Admin Organizational Unit for access to administrators. 
</p>
<br />

<p>

![5 new admin account](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/465990aa-babb-407f-8c1e-cc0366e72bcf)

</p>
<p>
You can then create new users to be added to your organizational units. Add an administrator so you can begin using an admin account. 
</p>
<br />

<p>

![6 new admin account2](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/36ed9b1e-322c-4f56-96d4-94675ad44e2b)

</p>
<p>
Add Domain Admins to the Security Groups so that you can begin adding permissions through an admin account. 
</p>
<br />

<p>

![7 create share files](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/0c9b534d-bbc8-4dcd-9333-e9603a88c6bd)

</p>
<p>
Create different share folders that you can now limit permissions to. 
</p>
<br />

<p>

![8 allow permissions](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/4a7144ca-8271-48af-975d-6138b06ae410)

</p>
<p>
From the Security tab in the folder settings you can set permissions to read and write access, read only access, or simply limit all access for certain users. 
</p>
<br />

<p>

![9 share with users](https://github.com/kylewilliamsrr/configure-ad/assets/144828759/9c06e5b4-07fd-4a9e-b5de-32da45287769)

</p>
<p>
You can also create share folders for specific departments. In this case, we create an Accounting folder and allow read and write permissions only for users that are apart of the Accounting Group. From here we can add as many groups and share folders with permissions as necessary to conduct normal business. 
</p>
<br />
