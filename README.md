<p align="center">

</p>

Inspecting Network and ICMP Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe icmp and network traffic to and from Azure Virtual Machines with Wireshark. <br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
<h2>Operating Systems Used </h2>

- Windows 10 (22H2)
- Ubuntu Server 22.04

<h2>High-Level Steps</h2>

- Step 1 Create a Resource Group
- Step 2 Create a Windows 10 Virtual Machine
- Step 3 Create a Linux (Ubuntu)


<h2>Creation Steps</h2>

1. Log into Microsoft Azure 1.a Click on Resource groups
![RG1](https://github.com/user-attachments/assets/33e1db8f-e218-45cc-82fd-ce185c2dc25c)
1.b click on + Create
![RGpic2](https://github.com/user-attachments/assets/57d1e2f4-b047-429a-8ceb-35c348662392)
1.c Inside the Resource group box type RG-Network-Activities or create your own name 1.d Inside of the Region box choose (Canada) Canada Central 1.e Click Review + create
![RGpic3](https://github.com/user-attachments/assets/007761e8-4cd6-4a7c-9445-7309f3c4f92e)
1.f Click Create
![RGpic4](https://github.com/user-attachments/assets/1ecb7e1b-32ae-4dc8-9c7f-0ed08d89717d)

2.Return back to the Home screen by clicking Home or Microsoft Azure in the top left corner 2.a Click on Virtual machines
![Windows1](https://github.com/user-attachments/assets/789e2887-05b3-414e-b057-aeacf7f30dc5)
2.b Click on +Create and select Azure virtual machine 
![Windows2](https://github.com/user-attachments/assets/2ab200f9-1e2e-43bc-a24a-6a6071759535)

2.c In the Resource group box select the Resource group that we /previously created (RG-Network-Activities) 2.d type windows-vm for the virtual machine's name 2. e In the Region box select the same Region you chose for your Resource group 2.f In the Image box choose Windows 10 Pro, version 22H2- x64 Gen2 2.g In the size box choose Standard D2s_13-2vcpus, 8GB memory and then scroll down to Administrator account section
![Windows3](https://github.com/user-attachments/assets/bcac51c7-c2a2-45ef-b41f-124044162aea)

2.h Create a Username and Password you will need this to log into your Virtual Machine 2.i Make sure to check the Licensing box 2.j Click Next: Disks
![Windows4](https://github.com/user-attachments/assets/3a9032ff-a82a-4612-a9e2-26494081773a)

2.k Click Next: Networking. 
![Windows5](https://github.com/user-attachments/assets/0900fa4b-e9da-49d3-9696-475bd19ef378)

2.l Click Create new to which will move you over to the right to create a new Virtual Network 2.m Type Lab2-Vnet to name your new virtual Network, and then click ok 2.n Click Review & create
![Windows6](https://github.com/user-attachments/assets/8d23203a-4f08-4790-9516-9754b57a0d6c)

2.o Once you see Validation passed click on Create 
once finished you'll see Your deployment is complete
![Windows7](https://github.com/user-attachments/assets/0b36fa7d-0d1e-4347-9675-7e2974de5dc2)

![Windows8](https://github.com/user-attachments/assets/de43cc8c-508d-4e21-87cb-e66887b3525e)

3. Return to the Home screen within Microsoft Azure 3.a Click on Victual machine
![Linux](https://github.com/user-attachments/assets/882253a8-b46a-4498-8c5d-5ddd889a2fe4)

3.b Near the top left of the screen click on + create, Azure virtual machine
![Linux1](https://github.com/user-attachments/assets/ff8bf459-595e-4f35-b77c-43a9e5a53928)
3.c In the Resource group box select the Resource group that we previously created (RG-Network Activities) 
3.d In the Virtual machine name box type linux-vm 3.e In the Region box select (Canada) Canada Central make sure you select the same Region as you did for your Resource group 3.f In the Image box select Ubuntu Server 22.04 LTS-x64 Gen2 3.g In the Size box select Standard-D2s_v3-2 vcpus 8 GiB memory and then scroll down to Administrator account
![Linux2](https://github.com/user-attachments/assets/9288f9f6-a7dd-4151-ac5c-23739a9b789f)
3.h Click on the circle for Password 3.i Create a Username and Password 3.j Click on Next: Disk
![Linux3](https://github.com/user-attachments/assets/ddb91de3-9da5-4e02-acec-12a695ed1a2e)
3.k Click on Next: Network
![Linux4](https://github.com/user-attachments/assets/41e02ce7-d5b1-4347-bf7e-4bf57b270b2d)
3.l In the Virtual network box select the Virtual network we created earlier when creating the Windows virtual machine 3.m Click on Review + create
![Linux5](https://github.com/user-attachments/assets/ba6a9123-2f79-4753-afba-0f178ec8c094)
3.n Click on Create and after a few minutes it will say your deployment is complete 
![Linux6](https://github.com/user-attachments/assets/e72f56eb-6e03-49ce-a64c-88819af32716)

![Linux7](https://github.com/user-attachments/assets/7d23e8a5-1200-42cb-a2f8-12d1eaa83fad)










