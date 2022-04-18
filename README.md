# <img src="https://user-images.githubusercontent.com/81617629/163785707-deed9383-3d8f-40ed-b5e2-c3f0662099ce.png" width="30"> Windows 10/11 Setup Guide
Step-by-Step Guide to setup a clean install of Windows (10/11)

***

> _**Following this guide will result in all of your data being wiped, so make sure to make a `BACKUP` of everything you need before following**_

***

- [Creating Installation Media](##Creating-Installation-Media)
- [Installing Windows](##Installing-Windows)
- [Setting UP Windows](##Setting-UP-Windows)

## Creating Installation Media

- [ ] Download [Windows](https://www.microsoft.com/en-us/software-download/) - Either Download the ISO Directly or Download the Media Creation Tool, and use it download and save the Windows ISO 
- Download [Rufus](https://rufus.ie/en/) 
- Connect a USB Device _(Make sure any data on it is backed up, as it will be formatted)_. Browse to the ISO by clicking on the `Select` button. The `Partition Scheme` should be the one your drive uses on which you plan to install Windows.
  - _(You can check the drives partition scheme by going into **Disk Management** by right-clicking on the **Windows Button** on the taskbar, then right-clicking on the drive you want to install Windows on, and going into **Properties**. You can see your Partition Style in the Volumes tab._)

     <img src="https://user-images.githubusercontent.com/81617629/163786938-d6a8417e-4701-4634-a7e0-9f3d6eeceabf.png" width="300">
    
- Set a name for the USB Drive, and click on Start. It will take a few minutes, and then your Bootable drive is ready.


## Installing Windows

- Access your BIOS by pressing your `BIOS Key` set by your manufacturer which could be `F1 F2 F10 F12 or DEL` during boot.
- Select the USB you just created, and boot from it. You will see something similar to below

     <img src="https://user-images.githubusercontent.com/81617629/163790441-3e0b95e1-10e6-4fc5-b886-e17f383509ee.png" width="450">

- Choose your Language and Other preferences and click `Next`. Then, click `Install Now`.
- You’ll be asked to activate Windows. Enter your product key or click `I don’t have a product key` if you’re reinstalling Windows.
- Select the operating system you want to install and click `Next`.
- Accept the license terms and click Next. Then, choose `Custom: Install Windows only (advanced)`
- See what Drive (if you have multiple) you want to Install Windows On. 
  - If the Drive you want to install on is currently in Use, you need to delete all the partitions of it until it looks someting similar to `Drive # Unallocated Space`. Then Select this unallocated space, and cick on `New`. If you want to separate your drive into multiple partitions, now is the time to do so, or you can just create the partition on which you install Windows on, and leave the other Unallocated space for later. Now click `Next`.
- Windows will begin to install. It might restart a couple times, that is Normal. When its done, it will ask for a final restart, after which you will be greeted by the Windows Setup Screen (Below picture is for Windows 11)

     <img src="https://user-images.githubusercontent.com/81617629/163792307-9de88fd8-1e97-430d-8acd-172063f174df.png" width="500">

- Go Through the Entire Setup, choosing the Correct `Keyboard Layout`, connecting to the `Wi-Fi`, logging into your `Microsoft Account`, and setting up a `Pin`. 
  - Set whatever Privacy settings you want _(I Recommend turning all of them off)_.
- You will end up on your Desktop, with everything set up and ready to go.

     <img src="https://user-images.githubusercontent.com/81617629/163793037-c8865794-3079-45e4-b959-3aa4e4d0780f.png" width="600">


## Setting UP Windows









