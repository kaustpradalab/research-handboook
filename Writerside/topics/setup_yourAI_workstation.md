# Set up your Ai workstation

This tutorial will guide you through configuring a workstation or server for AI projects from scratch. Since the author enjoys exploring the latest systems, the tutorial will use the installation of the latest version, Ubuntu 24.04, as an example.

## Install ubuntu in your computer or workstation

You can find the downloda link and new release here: <https://ubuntu.com/blog/tag/ubuntu-24-04-lts>,just download the version you like.
![downubuntu.png](downubuntu.png){width="400" }

After the download is complete, you'll need to use a USB drive (preferably a blank one) to create a bootable system disk.

If you are using **MACOS** you can follow  <xhttps://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-macos>

If you are using **WINDOWS** you can usen rufus <https://rufus.ie/zh/> and follow <https://ubuntu.com/tutorials/create-a-usb-stick-on-windows#1-overview>

I will follow the macos guide here.

Open the following app. 
![disk.png](disk.png){width="100" }
Find the **external** disk, and erase it:
![dickerase.png](dickerase.png){width="400" }
Download etcher <https://etcher.balena.io/#download-etcher>  in your device.
![etcher.png](etcher.png){width="400" }

then open this application:
![etcherteach.png](etcherteach.png){width="400" }

just 'flash' it.

Insert the USB drive into the new machine. Before the boot screen appears, repeatedly press F8 or F2 to enter the boot menu. Select USB (choose the **UEFI option**) as the boot device, and then boot Ubuntu from the USB drive. Follow the on-screen instructions to proceed.

Then just follow the guide here: <https://ubuntu.com/tutorials/install-ubuntu-desktop#4-boot-from-usb-flash-drive>

Finally you will have ubuntu 24.04LST in your workstation.

**Don't forget remove the USB drive before you restart your machine.**

## Install AI research application

Establishing an SSH Connection to Your Machine:

1. Check for Network Tools:

* Open the terminal on your workstation and enter `ifconfig`.

* If you receive a "command not found" error, it indicates that the network tools are not installed, and the SSH tool is likely missing as well.

2. Install SSH and Network Tool
`sudo apt install ssh` and `sudo apt install ssh net-tools` 

3. Connect via SSH:
Once installed, you can establish an SSH connection from another device using:

`ssh yourname@ip-of-yourworkstation` you can use `ifconfig`  to check the ip of your workstation