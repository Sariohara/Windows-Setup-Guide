# <img src="https://user-images.githubusercontent.com/81617629/163785707-deed9383-3d8f-40ed-b5e2-c3f0662099ce.png" width="30"> Windows 10/11 Setup Guide
Step-by-Step Guide to setup a clean install of Windows (10/11)

***

> ***Following this guide will result in all of your data being wiped, so make sure to make a `BACKUP` of everything you need before following***

***

## Step 1 - Creating Installation Media

1. Download [Windows](https://www.microsoft.com/en-us/software-download/) - Either Download the ISO Directly or Download the Media Creation Tool, and use it download and save the Windows ISO 
2. Download [Rufus](https://rufus.ie/en/) 
3. Connect a USB Device _(Make sure any data on it is backed up, as it will be formatted)_. Browse to the ISO by clicking on the `Select` button. The `Partition Scheme` should be the one your drive uses on which you plan to install Windows.
   - _(You can check the drives partition scheme by going into `Disk Management` by right-clicking on the **Windows Button** on the taskbar, then right-clicking on the drive you want to install Windows on, and going into `Properties`. You can see your Partition Style in the Volumes tab._)

     <img src="https://user-images.githubusercontent.com/81617629/163786938-d6a8417e-4701-4634-a7e0-9f3d6eeceabf.png" width="300">
    
4. Set a name for the USB Drive, and click on Start. It will take a few minutes, and then your Bootable drive is ready.

***

## Step 2 - Installing Windows

1. Access your BIOS by pressing your `BIOS Key` set by your manufacturer which could be `F1 F2 F10 F12 or DEL` during boot.
2. Select the USB you just created, and boot from it. You will see something similar to below

     <img src="https://user-images.githubusercontent.com/81617629/163790441-3e0b95e1-10e6-4fc5-b886-e17f383509ee.png" width="450">

3. Choose your Language and Other preferences and click `Next`. Then, click `Install Now`.
4. You’ll be asked to activate Windows. Enter your product key or click `I don’t have a product key` if you’re reinstalling Windows.
5. Select the operating system you want to install and click `Next`.
6. Accept the license terms and click Next. Then, choose `Custom: Install Windows only (advanced)`
7. See what Drive (if you have multiple) you want to Install Windows On. 
   - If the Drive you want to install on is currently in Use, you need to delete all the partitions of it until it looks someting similar to `Drive # Unallocated Space`. Then Select this unallocated space, and cick on `New`. If you want to separate your drive into multiple partitions, now is the time to do so, or you can just create the partition on which you install Windows on, and leave the other Unallocated space for later. Now click `Next`.
8. Windows will begin to install. It might restart a couple times, that is Normal. When its done, it will ask for a final restart, after which you will be greeted by the Windows Setup Screen (Below picture is for Windows 11)

     <img src="https://user-images.githubusercontent.com/81617629/163792307-9de88fd8-1e97-430d-8acd-172063f174df.png" width="500">

9. Go Through the Entire Setup, choosing the Correct `Keyboard Layout`, connecting to the `Wi-Fi`, logging into your `Microsoft Account`, and setting up a `Pin`. 
   - Set whatever Privacy settings you want _(I Recommend turning all of them off)_.
10. You will end up on your Desktop, with everything set up and ready to go.

***

## Step 3 - Getting Started

1. Update Windows to the Latest.
   - Go to `Settings` > `Windows Update` , and click on `Check for Updates`. It will Download and Install, multiple updates,  including the Graphics Driver (although it can be quite old, will fix this later) and other necessary drivers. 
   - You might need to check for updates a couple times, as it doesnt always download all of them at the same time.
   - When it has finished installing the updates, `Restart` the computer.
   - Now Go back to Windows Updates and Pause Updates for as long as possible.

2. If you have any drives or unallocated space that you would like to mount/create a partition of, you can go to `Disk Management` by right-clicking on the **Windows Button** on the taskbar. 
   - You will see all of your drives and/or unallocated spaces of any drives listed here. Right-Click on the Unallocated Space _**(usually marked with black shades)**_, and select `New Simple Volume`. Go through the setup, giving the Volume a Letter and Name. Click on `Finish`, and your drive/partition should show up in `This PC`.

3. Download and Install the [DirectX](https://www.microsoft.com/en-in/download/details.aspx?id=35) Web Installer.
   - This will install a number of runtime libraries from the legacy DirectX SDK for some games that use D3DX9, D3DX10, D3DX11, XAudio 2.7, XInput 1.3, XACT, and/or Managed DirectX 1.1. Note that this package does not modify the DirectX Runtime installed on your Windows OS in any way.

       <img src="https://user-images.githubusercontent.com/81617629/163797324-14a190de-cd5f-4301-9f2e-040e6440beb7.png" width="500">
             
4. Similarly, Go to the [Visual C++ Runtimes](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/) website. 
   - Select `Download` on the left side of the site, and select the `Server Closest to You`. The Download should begin.

       <img src="https://user-images.githubusercontent.com/81617629/163797741-bfad21ae-3757-4150-af6a-f06f2e4bc768.png" width="500">

   - Navigate to the folder where it downloaded. Extract all the contents into a folder. Run the `install_all.bat` files as Administration by right-clicking and selecting `Run as Administrator`.

5. This will make sure you have all the necessary software required to run **_most_** of the programs and games availaible on the internet. Most games will download nay missing softwares automatically.

6. Open `Settings`, Go to `Accessibility`
   - Go to `Mouse Pointer and Touch` > `Mouse` > `Additional Mouse Settings` > `Pointer Options` and unchecking `Enhance Pointer Precision`. Make sure the Pointer Speed is also set at 6/11

***

## Step 4 - Installing Drivers

### Graphics Driver. 

1. Go to either [Nvidia Official Drivers](https://www.nvidia.com/download/index.aspx) website or [AMD Official Drivers](https://www.amd.com/en/support) website and download your driver.
  
     <img src="https://user-images.githubusercontent.com/81617629/163810679-14211790-4784-4f06-871a-75ba4dd4b0dd.png">
       
     or
       
     <img src="https://user-images.githubusercontent.com/81617629/163811045-ecadc9f7-f238-433e-8573-62ac901ca4a2.png" width="500">

       
2. Download [Display Driver Uninstaller](https://www.guru3d.com/files-details/display-driver-uninstaller-download.html). Use this to fully uninstall the current installed driver and install the latest availaible.

   - Extract it to a folder.
   - Open run by `Win + R`, type `msconfig` and hit Enter. 
   - Go to the `Boot Tab` and Check `Safe Boot`. Click on Apply and Restart your PC.
   - When back on desktop, open DDU. When the dialog box opens, scroll to the bottom and turn on `Prevent downloads of drivers from "Windows Update" when "Windows" search for a driver for a device`
   - On the right side of the window, Select your `GPU`, and then either `NVIDIA` or `AMD`

       <img src="https://user-images.githubusercontent.com/81617629/163812602-213ebe41-4251-485c-ba30-14966114146e.png">

   - Click on `Clean and do NOT Restart`
   - When it has finished cleaning up, again open `MSCONFIG` (steps above) and uncheck `Safe Boot`. Click on Apply and restart your PC
   - When back on desktop, open the downloaded GPU driver, and go through the installation, unchecking anything you might not neend.
   - When finished installing, open DDU (no need for Safe Mode), click on `Options` and turn off `Prevent downloads of drivers from "Windows Update" when "Windows" search for a driver for a device`.


3. Set up the `Nvidia Control panel` with the recommended settings
   
   - Go to `3D Settings` > `Adjust Image Settings with Preview` and Select `Use Advanced 3D Image Settings`
   - Go to `Display` > `Adjust Desktop Size and Position` 
    - Set the Scaling mode to `Full-Screen` 
    - Set `Perform Scaling on` to `GPU` and turn on `Override the scaling Mode set the games and programs`
   - Go to `Display` > `Set up G-SYNC`
    - Enable G-SYNC, if you monitor supports it 


### CPU Drivers

- You can download your CPU drivers by going to either [AMD's](https://www.amd.com/en/support) website OR [Intel's](https://www.intel.com/content/www/us/en/products/details/processors/core.html).
  - Just download the driver specific for your CPU and run the driver files, and restart at the end.


### More Drivers

1. Apart from the GPU and CPU drivers, you need to download the drivers recommended by your Motherboard/System Manufacturer
2. These Generally include drivers like `Sound` , `Networks` , and/or some applications. 
3. You can also download and update your `BIOS` by getting the newer versions from your manufacturers website, and installing it, though it is not recommended as it can be quite complicated. If everything is already running fine, there is no need to update BIOS, unless there are some security updates included in it

***

## Step 5 - Windows Settings

Open `Settings`, and set up any and everything you want according to your preferences. A few settings I recommend switching are : 

1. Go to `System` 
   - Go to `Display` and set the `Display Resolution` to the Highest Availaible. Also Go to `Advanced Display` and set the Refresh Rate to the Highest Availaible.
   - Go to `Notifications` and turn off notifications from any app you dont want.
   - Go to `Multi-tasking` and set the `Alt + Tab` button only shows `Open Windows Only`.
    
2. Go to `Personalisation`
   - Go to `Colours` and set the mode to `Light` or `Dark`. You can also turn off `Transparency Effects` here. 
   - Go to `Start`
     - Turn off `Show Recently Added Apps`
     - Turn off `Show Recently opened items in Start, Jump Lists, and File Explorer`
     - Go to `Folders` and uncheck everything except `Settings` and `Personal Folder`  
   - Go to `Taskbar`
     - Turn off all the `Taskbar Items` (Leave Search button on if you want)
     - Turn off all the `Taskbar Corner Items`
     - Turn on/off what you want in `Taskbar Corner Overflow`
     - Set `Taskbar Behaviours` to personal preference.
      
3. Go to `Apps`
   -  Go to`Apps & Features` 
      - Set `Choose where to get apps` to `Anywhere`
      - Uninstall all the apps you dont need like `OneDrive` , `Skype` , `Films` , `Groove Music` , `Tips` etc. You can also use a third party tool like [Bloatbox](https://github.com/builtbybel/bloatbox).
   - Go to `Offline Maps` and turn off Auto Updates of Maps
   - Go to `Startup` and turn off all of the apps you want want runned when you start your PC. Leave `Realtek HD Audio Universal Service` to ON if present.

4. Go to `Accounts`
   - Go to `Sign-in Options`
     - Turn off `Automatically save my Restartable apps and restart them when I sign back in`
     - Turn off `Show my account Details such as my email address on the sign-in screen`
     - Turn off `Use my sign-in info to automatically finish setting up after an update`
   - Go to `Windows Backup`
     - Turn off `Remember my apps`
     - Turn off `Remember my preferences`

5. Go to `Time & Language`
   - Go to `Date & Time` and turn on `Set the time Automatically`. Also set the correct `Time Zone`
   - Go to `Language & Region`
     - Set the `Windows Display Language` to your preferred language.
     - Set the `Country or Region`
     - Set the `Regional Format` to the correct one, click on the down arrow and click on `Change Formats`, and set it according to your preferences.
   - Go to `Typing`
     - Turn off `Show Text Suggestions when Typing`
     - Turn off `Multilingual Text Suggestions`
     - Go to `Advanced Keyboard Settings`. Check the `Use the Desktop Language bar When it is availaible`. Click on `Language bar options`. Uncheck everything and set Language bar to `Hidden`.
      - Setting this up removes the ***Language Input Indicator*** from the Taskbar, very annoying otherwise.

6. Go to `Gaming`
   - Click on ***Xbox Game Bar*** and turn off `Open Xbox Gamebar Using this button on a controller`
   - Click on ***Game Mode*** and turn on `Game Mode`

7. The `Privacy and Security` is all personal preference, but I recommend turning off everything you dont need. Just make sure to not fully turn off all of them, only disable what you know you dont need.

- You can also set up almost all of these settings by using another utility [ThisIsWin11](https://github.com/builtbybel/ThisIsWin11). You can also download multiple applications directly through this using Windows Package Manager (You Will Need WinGet for this, the app will guide you to install it)

***

## Step 6 - Finishing Up

At this point, almost everything is set up and ready to go. Things recommended at this point - 

1. Cleanup your Drives
   - This can be done through either `Disk Cleanup` (Can be opened by searching ***Disk Cleanup***), a built in Windows Utility, or you can use a third party program like [BurnBytes](https://github.com/builtbybel/burnbytes)
 
        <img src="https://user-images.githubusercontent.com/81617629/163946826-86b59f3c-7c60-470d-a6cc-a38fb99ded46.png">

 
   - Both are pretty straight forward. Open whichever one you want to use, select the drive you want to clean up, and select everything you wish to delete. This generally includes stuff like `Windows Update Cleanup` , `Temporary Files` , `Delivery Optimization Files`. 
   - Be careful in what you select, as there is an option to clear out `Downloaded Files` , and this will remove everything from your 'Downloads' folder.

2. Create a Restore Point
   - Now that Windows has been set up in the optimal way, you should create a system restore point, so if at any point in the future you need to revert back without doing everything from scratch again, you can use this.
   - Search for ***Create a Restore Point*** and open the app. 
   - Select the Drive on which you Installed Windows and click `Configure`
   - Make sure `System Protection` is turned `On` and Disk Usage is set to around `10 GB`. Click on `Apply` and close.

     <img src="https://user-images.githubusercontent.com/81617629/163949999-f515397c-ece2-4bde-9049-2426b3a56259.png">

   - Select `Create` button at the bottom of the dialog box. A new Window will open, put in a name for your Restore Point. Date and Time are added Automatically, and click `Create`. It will take a minute, and then it will finish. Thats it.

3. Installing Apps
   - You can download any and all apps you require from their respective websites. You can also use [Ninite](https://ninite.com/) to make the process a lot simpler. Just select the apps you want, and click on `Get Your Ninite` at the bottom of the page. This will download a custom installer which will install/update all the apps you selected.
   - Some Recommended Apps are - [Steam](https://store.steampowered.com/about/) , [Discord](https://discord.com/) , [qBittorrent](https://www.qbittorrent.org/download.php) , [MSI AfterBurner](https://www.msi.com/Landing/afterburner/graphics-cards) , [WinAero Tweaker](https://winaero.com/download-winaero-tweaker/) , and [ShareX](https://getsharex.com/)

***

## Step 7 - Optional but Recommended Stuff

1. Nilesoft Shell
   - In Windows 11, Microsoft Introduced a new context menu (Menu that opens when you right-click). The problem with this is that even though it looks nicer, it has moved a lot of stuff around, making the basic functionality a lot more tedious.
   - Fortunately, ***Shell*** is a context menu extender, that not only looks identical, but is a lot more powerful.
             
        <img src="https://user-images.githubusercontent.com/81617629/163951766-540937ff-ebf2-4c0c-9615-68a402dda5b4.png">
        
   - You can handpick the items to integrate into Windows File Explorer context menu, create custom commands to access all your favorite web pages, files, and folders, and launch any application directly from the context menu.
handpick the items to integrate into Windows File Explorer context menu, create custom commands to access all your favorite web pages, files, and folders, and launch any application directly from the context menu.
   - Setting it up is pretty simple. **Download** the zip file (32-bit or 64-bit) > **Extract** > Cut and Paste it to a safe place (Like ***Program Filex***) > Run the `Shell.exe` as `Administrator` > `Register`.
   - The Windows Explorer will restart, and you will have a brand new Context Menu.
   - You can edit everything here through the `shell.shl` file located in the directory of this application. Open it with `Notepad` and set it up however you like. I have created a custom [shell.shl](https://www.mediafire.com/file/j41xv1w8a9sgqb2/shell.shl/file) for the version 1.5, for my personal use. You dont need to use it.
   - Whenever you edit stuff in the `shell.shl`, make sure you restart the explorer. You wont see the changes you made otherwise.
   - You can also revert to the Windows 10 Context Menu by following [this](https://www.tomshardware.com/how-to/restore-windows-10-explorer-windows-11) guide, but there are some highlighting issues that I faced so I Wouldnt Recommend it.

2. Messing with the Registry

   > ***This next part includes making changes to the registry of Windows. If you are not comfortable doing this, avoiding this step is recommended.***
   
   - Make a backup of Registry first before proceeding. Incase something breaks, you can use this file to restore the registry to the default state. 
     - Open Registry Editor by typing `regedit` in Run `Win + R`
     - At the top left corner, Click `File` > `Export`. Save the backup in a safe place.

   -  Some basic Registry Tweaks. Download [this](https://www.mediafire.com/file/mzq4qrvt38wknqi/RegTweaks.reg/file) file. You can see what changes this will make to the registry by Right-Clicking on this file and clicking `Edit`
      - This disables things like `Power Throttling` , `Network Throttling` ,  `Games Scheduling` , `Automatic Maintainence` and `Menu Show Delay`
     
   - Gamebar
     - By Default, Windows 11 does not have any option to disable Gamebar. All you can do is stop the controller button from opening GameBar
     - Use [this](https://www.mediafire.com/file/tte1yfp9kgzofiu/Disable_Gamebar.reg/file) to `Disable` GameBar.
     - Use [this](https://www.mediafire.com/file/gg9a8ih840m376l/Enable_Gamebar.reg/file) to `Enable` GameBar.

***
