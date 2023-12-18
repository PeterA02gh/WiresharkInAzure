<h1>Let's begin by creating our resource group!</h1>

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
    it isn't already. Name it 'VM1' and put it inside the same region as the Resource Group. For the size, the smallest should
    work fine for this lab. Let's give ourselves a username and password for this virtual machine.
    
    ‼️Write it down! You will need it later to Remote Desktop into it!‼️
    
<p>
<img src="https://i.imgur.com/B0zB7nn.png" alt="Creating our Windows 10 VM"/>
</p>

    Click and confirm the licensing at the bottom of the page. Now go from the 'Basics' tab and skip to the 'Networking' tab. 
    You will see some choices for how the Virtual Machine handles networking. Hover to 'Virtual Network' and click 'Create new'.
    Create a vnet and name it 'RG-Lab-1-vnet'. We will be using this vnet for both of the virtual machines.

<p>
<img src="https://i.imgur.com/n6hXrV1.png" alt="Creating our Windows 10 VM"/>
</p>

    After that, the virtual machine is now ready to be deployed! Click create and allow it to process.
    In the meantime, we can create our Linux server virtual Machine.
