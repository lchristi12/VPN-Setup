<p align="center">
<img width="225" height="225" alt="image" src="https://github.com/user-attachments/assets/81c5541a-92d7-4f7c-97c4-df03e9018cc3" />


</p>

<h1> VPN Setup in Virtual Machines</h1>
This tutorial outlines the prerequisites and using a VPN within the VM and your personal computer.<br />





<h2>Environments and Technologies Used</h2>

- Remote Desktop
- Microsoft Azure (VMs/Compute)
- VPN (Proton VPN)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1 Identify Local IP address
- Step 2 Setting up VM using Azure
- Step 3 Identify IP address on VM (Virginia)
- Step 4 Connect VPN through the VM
- Step 5 Identify IP address using VPN (Netherlands)

<h2>Installation Walkthrough</h2>
<p> Step 1 
<p> Locate your personal IP address by using the  https://whatismyipaddress.com. This site will show your local IP address and will be used though this tutorial. See example below.


<img width="700" height="394" alt="Screenshot 2025-09-08 172310" src="https://github.com/user-attachments/assets/4b8bd6eb-ff03-4772-a0fa-55a5aa700986" />

 </p> Step 2
 </p> Next, we will create and set up a Virtual Machine.
 </p> Go to www.portal.azure.com, in the search bar type Virtual Machines and click on create.
 </p> Make sure you create a free account that will have 200 dollars in credit to work with throughout the tutorial.
<img width="1940" height="1110" alt="Screenshot 2025-09-11 003632" src="https://github.com/user-attachments/assets/7cac4c7f-8cc7-4097-b74a-51046dbbeb45" />

</p> On this page, create a resource group and name is vpn-test (for the sake of the tutorial). Next, name the VM vpn-test-win-10  
</p>Make sure the correct region is selected, in this case, East US 2. See example below.
<img width="500" height="333" alt="Screenshot 2025-09-08 170610" src="https://github.com/user-attachments/assets/3dfc006f-29cc-4e89-85e7-f64051dc26ce" />


<p> Next, for the image, click on the Windows 10 Pro, version 22H2- x64 Gen2 which the OS (operating system) that will be used. For the size, select Standard _D2s_-2 vcpus, 8 GiB Memory. 
<p>Under Administrator Account, enter your own username and password. 
<p>Check the box under Licensing and click review and create.
<img width="480" height="679" alt="Screenshot 2025-09-08 170718" src="https://github.com/user-attachments/assets/dc825ca4-d93f-495d-b713-9264089cc9a2" />

</p> Step 3 
</p> First locate the public IP address on the Virtual Machine that was created. Click on the virtual machine and on the right side of the page should be where the public IP address is located. See example below.
</p> Next, we are going to connect to the Virtual Machine by using the program, Remote Desktop Connection. Enter username and password and you should be able to connect to the Virtual Machine.
</p> Once logged into the VM, go into the web browser and search the site, https://whatismyipaddress.com, and look up the local IP address of the VM. For the tutorial, the IP address is located in Virginia. See example below.
<img width="1910" height="580" alt="Screenshot 2025-09-08 181205" src="https://github.com/user-attachments/assets/d412e40b-290e-4ff2-aeae-44c40d897225" />
<img width="500" height="487" alt="Screenshot 2025-09-08 181106" src="https://github.com/user-attachments/assets/4b7baee3-b1b2-4491-b112-7f04cf2e23ad" />
<img width="2000" height="1124" alt="Annotation 2025-08-31 002901" src="https://github.com/user-attachments/assets/6d4e021d-a0f9-46ce-9068-cdbf896bcdbb" />





<img width="1300" height="742" alt="Screenshot 2025-09-08 172919" src="https://github.com/user-attachments/assets/559f212b-7019-41e6-b5cb-ec5e65aeaf29" />

<p> Step 4

</p>Create a VPN account (Proton) and connect to VPN
<p> Go to the web browser and search www.protonvpn.com and create a free account. Click on the download tab and choose the windows version. Follow the prompts. When the installation is finished, log in Proton using the information to create the account. After, connect to the VPN.
 
<img width="300" height="422" alt="Annotation 2025-09-08 213947" src="https://github.com/user-attachments/assets/71562067-fc5d-457e-9b65-5c957100a336" />

<img width="1000" height="562" alt="Annotation 2025-09-08 214059" src="https://github.com/user-attachments/assets/f6d8cbbf-ff58-4251-b992-69e9c2b77e43" />

<img width="700" height="446" alt="Annotation 2025-09-08 215225" src="https://github.com/user-attachments/assets/0310ff84-edd4-4d0f-b8d8-c9f66bee12d2" />

</p>
<p>
Once you are logged on, you can choose where your VPN to be located in. For quicker connection, click "connect" and the website will choose a country for the VPN to be in.
<img width="2200" height="1165" alt="Annotation 2025-09-08 215531" src="https://github.com/user-attachments/assets/290ca545-3e4c-4641-8d0a-4d157e7c2b7a" />
<p> For the sake of this tutorial, the VPN location chosen was in the Netherlands. Next, we will observe the the IP address again after connecting the VPN to the Netherlands. Use the VM browser to search the site  www.whatismyipaddress.com and it will show different IP address from where we started. It will show the country where your VPN is connected to.
 
 <img width="2000" height="1046" alt="Annotation 2025-09-08 215903" src="https://github.com/user-attachments/assets/bb7432c1-2d8b-45f1-8bf9-d588ba515261" />

<img width="1778" height="758" alt="Annotation 2025-09-08 220442" src="https://github.com/user-attachments/assets/a8a10f61-22a3-4c91-bc47-42dd410ac863" />


<p> In conclusion, we have used different IP addresses from our local PC to connect to the interent. VPNs could be very useful for browsing the internet, working from home, or even streaming movies and shows. Hope you found this tutorial helpful. If you are finished, make sure you go to the azure portal and delete the VM so no additional charges will apply to your account.
<br />
