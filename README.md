<!-- TOC --><a name="this-is-still-wip"></a>
# THIS IS STILL WIP

<!-- TOC --><a name="table-of-contents"></a>
## Table of Contents
   * [Disclaimer](#disclaimer)
   * [Introduction](#introduction)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
      + [Step 1: Download the ISO](#step-1-download-the-iso)
      + [Step 2: Create a Live USB](#step-2-create-a-live-usb)
      + [Step 3: Boot Arch Live ISO](#step-3-boot-arch-live-iso)
      + [Step 4: Set Keyboard Layout](#step-4-set-keyboard-layout)
      + [Step 5: Enable Internet Connection](#step-5-enable-internet-connection)
      + [Step 6: Enable Network Time Protocols (NTP)](#step-6-enable-network-time-protocols-ntp)
      + [Step 7: Partition the Disks](#step-7-partition-the-disks)
      + [Step 8: Create Filesystem](#step-8-create-filesystem)
      + [Step 9 Check the Mirror List for an Appropriate Mirror](#step-9-check-the-mirror-list-for-an-appropriate-mirror)
      + [Step 10: Install Arch Linux](#step-10-install-arch-linux)
      + [Step 11: Configure Arch Linux](#step-11-configure-arch-linux)
      + [Step 12: Install Grub Bootloader](#step-12-install-grub-bootloader)
      + [Step 13: Create a New User and Set Up Previleges](#step-13-create-a-new-user-and-set-up-previleges)
      + [Step 14: Exit Arch-Chroot Environment and Reboot](#step-14-exit-arch-chroot-environment-and-reboot)
      + [Step 15: Login to Arch Linux](#step-15-login-to-arch-linux)


<!-- TOC --><a name="disclaimer"></a>
## Disclaimer
I’m not an experienced Arch user by any means—this is just a fun project for me. I’m not responsible for any data loss or hardware damage that might occur. If you don’t know the basics of Linux, it’s best not to follow my guide.

The guide below covers Arch installation without dual-booting with Windows or any other operating systems.

<!-- TOC --><a name="introduction"></a>
## Introduction

Arch Linux is widely recognized for its versatility and low system requirements, making it one of the most popular Linux distributions. With its rolling release model, users consistently have access to the latest Linux kernel and software updates.

<!-- TOC --><a name="prerequisites"></a>
## Prerequisites
- At least 1GB of RAM and 20GB of storage spaces.
- Internet Connection
- USB Drive with at least 4GB of free space for the ISO Image

<!-- TOC --><a name="installation"></a>
## Installation
Installing Arch Linux from scratch grants you full control over what gets installed, enabling you to customize the system to your specific needs. The installation process also deepens your understanding of Linux, from disk partitioning to bootloader (GRUB) configuration.

The result is a minimal installation, free from unnecessary software, which enhances system performance. Follow the steps below to install Arch Linux.

<!-- TOC --><a name="step-1-download-the-iso"></a>
### Step 1: Download the ISO
Download the ISO from the [Arch Linux Download Page](https://archlinux.org/download/). There are two methods to do this:
- BitTorrent
- Direct Download

To download the ISO via torrent, you can either add the magnet link to your BitTorrent app of your choice or download the torrent file directly. Alternatively, scroll down the page to find a mirror closest to your location and download the ISO file from there.

![image](https://github.com/user-attachments/assets/5a00f30a-d00f-4b23-87cc-03f5f6babab5)

<!-- TOC --><a name="step-2-create-a-live-usb"></a>
### Step 2: Create a Live USB
After obtaining the Arch Linux ISO file, create a live USB

The easiest way to create an Arch Linux live USB is by using a tool like Etcher GUI, which is available for both Linux and Windows systems.

If you are using a Linux system, you can create a live USB using the [dd](https://www.geeksforgeeks.org/dd-command-linux/) command.
``` 
dd bs=4M if=/[path_to_arch.iso] of=/dev/[path_to_usb_device] status=progress && sync
```
For example:

```
dd bs=4M if=/home/frostlynn/Downloads/archlinux.iso of=/dev/sdX status=progress && sync 
```

<!-- TOC --><a name="step-3-boot-arch-live-iso"></a>
### Step 3: Boot Arch Live ISO

Start the installation by booting up Arch Linux from the installation media created before.
1. Insert the installation media into your PC or Laptop and restart.
2. Depending on your system, press **F2**, **F10**, **F12**, or **Delete** to enter the boot menu and select the device from which the system will boot.
3. Select the preferred installation media you created in the previous step. The following screen will appear after Arch boots.
   
   ![image](https://github.com/user-attachments/assets/786b4df3-2d37-49c7-885e-b0dc107d801e)

Select **Arch Linux install media (X86_64, BIOS)** and press **ENTER** to begin the setup.

<!-- TOC --><a name="step-4-set-keyboard-layout"></a>
### Step 4: Set Keyboard Layout

<!-- TOC --><a name="step-5-enable-internet-connection"></a>
### Step 5: Enable Internet Connection

<!-- TOC --><a name="step-6-enable-network-time-protocols-ntp"></a>
### Step 6: Enable Network Time Protocols (NTP)

<!-- TOC --><a name="step-7-partition-the-disks"></a>
### Step 7: Partition the Disks

<!-- TOC --><a name="step-8-create-filesystem"></a>
### Step 8: Create Filesystem

<!-- TOC --><a name="step-9-check-the-mirror-list-for-an-appropriate-mirror"></a>
### Step 9 Check the Mirror List for an Appropriate Mirror

<!-- TOC --><a name="step-10-install-arch-linux"></a>
### Step 10: Install Arch Linux

<!-- TOC --><a name="step-11-configure-arch-linux"></a>
### Step 11: Configure Arch Linux

<!-- TOC --><a name="step-12-install-grub-bootloader"></a>
### Step 12: Install Grub Bootloader

<!-- TOC --><a name="step-13-create-a-new-user-and-set-up-previleges"></a>
### Step 13: Create a New User and Set Up Previleges

<!-- TOC --><a name="step-14-exit-arch-chroot-environment-and-reboot"></a>
### Step 14: Exit Arch-Chroot Environment and Reboot

<!-- TOC --><a name="step-15-login-to-arch-linux"></a>
### Step 15: Login to Arch Linux