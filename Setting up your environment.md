# Let's begin by creating our resources!

    Go to portal.azure.com. There are a wide variety of options to click on, but go ahead and click on 'Resource Groups'.

<p>
<img src="https://i.imgur.com/7krsaNf.jpg" alt="Click on resource group"/>
</p>

    Let's name it 'RG-Lab-1' and put it in our region of choice. I chose (US) West US 2 because it's the closest to me.

<p>
<img src="https://i.imgur.com/sKuqDgB.jpg" alt="Creating our resource group"/>
</p>

    We can go ahead and create our resource group. There are other options that we can adjust but they are not important to our lab.

    Next, we will be using two virtual machines. One will be running Windows 10 and the other will be using a Linux Server (Ubuntu).

    We can go to Virtual Machines by typing 'Virtual Machines' into the search bar or by clicking on the 'Virtual Machines' tab on
    the homepage. Let's make our Windows 10 VM.

    It should be under our Azure subscription and inside the Resource Group we made earlier. Put it inside the Resource Group if
    it isn't already. Name it 'VM1' and put it inside the same region as the Resource Group. For the image, use Windows 10 (22H2).
    For the size, the smallest should work fine for this lab. Let's give ourselves a username and password for this virtual machine.
    
    ‼️Write it down! We will need the username and password later to Remote Desktop into VM1!‼️
    
<p>
<img src="https://i.imgur.com/B0zB7nn.png" alt="Creating our Windows 10 VM"/>
</p>

    Click and confirm the licensing at the bottom of the page. Now go from the 'Basics' tab and skip to the 'Networking' tab. 
    You will see some choices for how the Virtual Machine handles networking. Hover to 'Virtual Network' and click 'Create new'.
    Create a vnet and name it 'RG-Lab-1-vnet'. We will be using this vnet for both of the virtual machines.

<p>
<img src="https://i.imgur.com/n6hXrV1.png" alt="Creating our VNET"/>
</p>

    After that, the virtual machine is now ready to be deployed! Click create and allow it to process.
    In the meantime, we can create our Linux server virtual Machine. Create another virtual machine and follow the same processes
    but this time name it 'VM2'and image it with Ubuntu Server 20.04.

<p>
<img src="https://i.imgur.com/6CDP1nm.png" alt="Creating our Ubuntu Server VM"/>
</p>

    Rather than have the 'Authentication type' be set to SSH public key, let's change it to password. It will prompt for a username
    and password just like VM1. Did you remember to write it down?

<p>
<img src="https://i.imgur.com/hSTqfiW.png" alt="Setting our Ubuntu Server VNET"/>
</p>

    Just like VM1, set the virtual network of the Ubuntu server to RG-Lab-1-vnet. We want both VM's on the same virtual network.
    It would be like two computers connected to the same router but on different

<p>
<img src="https://i.imgur.com/16Zmk36.png" alt="Setting our Ubuntu Server VNET"/>
</p>

    We now have both virtual machines ready for the lab to use! Let's connect to the Windows 10 VM using Remote Desktop Connection. 
    First, go to VM1 under 'Virtual Machines' and find it's public IP address. 
    Open up Remote Desktop by searching for Remote Desktop in the start menu search bar. Paste VM1's public IP address into RDP. 
    It will now prompt you for the username and password we set earlier.

<p>
<img src="https://i.imgur.com/N8QRGC0.png" alt="Setting our Ubuntu Server VNET"/>
</p>

    The virtual machine will now ask us how we'd like to set up our new Windows 10 operating system. 
    We can just ignore this and go straight to the new operating system. 
    Our next step is getting Wireshark set up on VM1. Let's open up Microsoft Edge and download Wireshark from it's official website.

<p>
<img src="https://i.imgur.com/N8QRGC0.png" alt="Setting our Ubuntu Server VNET"/>
</p>

    Download the Windows x64 installer. Click yes to all until Wireshark is finished installing.
    Congrats! We now have our environment set up for this lab!.
