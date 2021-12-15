**Virtualization**
* A replication of hardware to simualte a virtual machine inside a physical machine
* Two Types of Virtualization:
  * Server-side virtualization
  * Client-side virtualization

**Server-side Virtualization**
Virtual Desktop Infrastructure (VDI) 
* Thick/fath client
* Thin client
* Zero client

**Client-sidee Virtualization**
* Software that can be installed on a computer to manage virtul machines
* VMs can have their own OS installed
* To be able to run a client-side virtualization:
* Hypervisor
  * hardware support
    * capable cpu
    * enough ram
    * enough storage

**Type 1 vs Type 2 Hypervisor**
*Type 1*
* runs on hardware
  * VMware ESX and ESXi
  * Citrix XenServer

*Type 2*
* runs on a host operating system
  * VMware
  * Oracle VirtualBox

**Benefits of Virtualization**
* Can run multiple OSs on one machine
* Allows applications to be tested before installing them onto the host machine
* Reduces costs by decreasing the physical hardware needed that get purchased on a network
* allows access to experiment with any untested programs without directly damaging the host machines

**VirtualBox**
* A type 2 virtualization product for enterprise/home use
* Runs on:
  * Windows
  * Linux
  * Macintosh
  * Solaris

**VMWare Workstation Player**
* Free of charge, type 2
* free version of Workstation but is restricted
* Available nn Linux and Windows
* Can support a big amount of guest OSs

**Requirements for Computer Virtualization**
* AMD V or INTEL V compatible processor
* Dual core x64 processor with 1.3 GHz or faster 4GB of RAM
* Enough free hard drive space for installing guest OSs

**Using Virtualbox**
* Step 1: download the current version of Viirtualbox
* Step 2: go to where it says "new" and create a machine 
  * have it have ubuntu in the name so Virtualbox can automatically recognize that the OS that is to be downloaded is of Ubuntu
* put whatever MB of ram that the OS can use, recommeded 4 MB of ram
  * In the settings where it says *System* the base memory is also where you can edit the amount of MB that can be used from the ram.
* next would be making sure it is a VDI machine
* after you would proceed to put the amount of storage the VM would need, recommended 2-4 GB or at least 1/4 of what the actual computer has

**Powerpoint 3**
**Installing Ubuntu 20.04**
* start the virtual machine and make sure it has Ubuntu in the name so that it can immediantly recognize it will be an Ubuntu VM
* recommended 2 GB of ram or at least 4 MB if it is for just 1 VM
* Next click, Create a virtual hard disk now, which indicates any size can be used
* Next would be VDI (VirtualBox Disk Image), which formats the image
* Dynamically allocated isn't as bothersome and will use actual storage from the hard drive
* recommended GB for Ubuntu is 25 GB
* in General settings after completing you would go in and make sure it has bidirectional selected. It allows ability to copy and paste between Guest and User.
* Only give your VM a good quantity of RAM
* the amount the host CPU to Virtual CPU should be unlimited
* The virtual graphics card can also be selected to the amount of memory provided.
* IDE controller would be where the Optical disks are attached, they would be downloaded in the physical computers folders
* after everything has been set up, user can proceed to click start and wait for the OS to boot up.
* click start
* click install ubuntu 
* Will be prompted to the Welcome Screen
  * pick main language the VM will use
  * normal installation, download updates + install third party much be checked.
  * next click erase disk
  * next will be prompted to click ok because the partitions will be formatted
  * after you may pick where you are in the world
  * following this, you will be prompted to put in basic user information like computer name and user/passwords
* after installation is complete, it will prompt you to restart the VM

Class preparations
Ubuntu Software update : sudo apt update; sudo apt upgrade -y; sudo apt full-upgrade -y

or sudo apt update && sudo apt upgrade -y

or... do this all on one single line: sudo apt install curl -y; curl https://raw.githubusercontent.com/ra559/cis106/main/guides/oneliner.sh | bash

**What is a Raspberry Pi?**
A raspberry pi is a low cost, credit-card sized computer that plugs in to a monitor or Tv and can use a regular keyboard and mouse. It is a tiny computer that functions as a regular desktop
* The main components needed to use a raspberry pi would be:
  * The raspberry Pi itself
  * the Pi Case
  * Pi Power Supply
  * Micro SD
  * HDMI Cable
* You would need to use an imager to download whatever OS is needed into the raspberry Pi on the Micro SD

**Working with Raspberry Pi OS**
* The steps that are included in the welcome screen of the Raspberry Pi OS is 
  * Click next to get started
  * Set the country and language
  * set a password
  * connect raspberry pi to the wifi
  * the software will be updated and checked before using 
  * onces it's done, the wizard will restart the OS and have it running

**Different Operating Systems for the Raspberry Pi**
* Ubuntu
* Kali Linux
* Diet Pi
* Arch Linux
* Elementary OS
* Manjaro
* Windows 10 
* Android


