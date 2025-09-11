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
</p> Once logged into the VM, go into the web browser and search the site, https://whatismyipaddress.com, and look up the local IP address of the VM. See example below.
<img width="1910" height="580" alt="Screenshot 2025-09-08 181205" src="https://github.com/user-attachments/assets/d412e40b-290e-4ff2-aeae-44c40d897225" />
<img width="500" height="487" alt="Screenshot 2025-09-08 181106" src="https://github.com/user-attachments/assets/4b7baee3-b1b2-4491-b112-7f04cf2e23ad" />
<img width="2000" height="1124" alt="Annotation 2025-08-31 002901" src="https://github.com/user-attachments/assets/6d4e021d-a0f9-46ce-9068-cdbf896bcdbb" />





<img width="1300" height="742" alt="Screenshot 2025-09-08 172919" src="https://github.com/user-attachments/assets/559f212b-7019-41e6-b5cb-ec5e65aeaf29" />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
