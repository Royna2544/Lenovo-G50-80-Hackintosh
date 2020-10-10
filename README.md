# Lenovo-G50-80-Opencore-v0.6.2(Offical Ver.)
# Introduction
This is the EFI folder for installing hackintosh in Lenovo G50-80. I made it from scratch. For people who want to know how to make the EFI folder for their computer, refer to the wiki (Will be added ASAP)
# Lenovo G50-80 Basic Specs:
Type: Laptop

CPU: Intel Core i5-5200U @ 2.2Ghz (Turbo Clock up to 2.7GHz)

GPU: Intel HD Graphics 5500 

RAM: Samsung DDR3 8GB (1600MHz)

Audio: Conxeant SmartAudio HD (Codec CX20751)

Touchpad: ELAN Pointing Device

Disk: WD Green SSD 240GB

Ethernet: Realtek RTL8168GU/8111GU PCI Express Gigabit Ethernet

Wifi: Qualcomm Atheros AR9565 Wireless Network Adapter (See HowToEnableQcomAtherosWiFi.md)

Bluetooth: Qualcomm Atheros Bluetooth 4.0 (Currently not working)

WebCam: Lenovo EasyCamera

ThunderBolt Ports: N/A

# Current Status: Working & Not Working
1. Hardware Video Decoding : Fully Supported
2. Audio : Fully Working
3. WebCam: Fully Working
4. Card Reader : It is natively not supported by Apple, therefore not working
5. CD-Rom Reader&Writer : Fully Working
6. Ethernet : Working on full speed
7. Battery Percentage : Haven't tested. I don't have battery in my laptop
. I lost it
8. SSD/HDD : Fully Working
9. USB : Fully Working
10. Bluetooth & WiFi : Doesn't work. I may have to find some kexts for them to work.
# Installation
1. From a real Mac or VM, Get the Install macOS xxx.app. Google it for details (xxx is the version of macOS you want to install on your non-mac PC)
2. Put the app to /Applications
3. Insert a USB to Mac or VM and connect it. Take note of the USB name. 

4-1. execute "sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/(Your USB device name) (If you want to install macOS Catalina)

4-2. execute "sudo /Applications/Install\ macOS\ Big\ Sur\ Beta.app/Contents/Resources/createinstallmedia --volume /Volumes/(Your USB device name) (If you want to install macOS Big Sur Beta)

5. Enter password of root (WARNING: THIS WILL WIPE DATA ON THE SELECTED DRIVE. BE EXTRA CAREFUL)
6. Wait until the making of bootable macOS Drive finishs 
7. Mount the USB's EFI using ESP Mounter Pro or any other EFI mounter, copy and paste the EFI Folder in releases page. (Note : the structure should be /EFI/EFI/OC, /EFI/EFI/BOOT)
8. In the PC that you want to run Macintosh, enter Boot Menu and boot from USB
9. As some texts passes, just wait.
10. If the installer appears, then you're in the right place. Go to disk utility and Wipe the Disk as APFS. (WARNING: THIS WILL WIPE DATA ON THE SELECTED DRIVE. BE EXTRA CAREFUL)
11. Exit the disk utility and install macOS as instructed.
12. The computer will reboot 2~3 times. This is very normal and just select 'preboot' on every bootloader menu. 
13. If it was successful, the mac setup screen will appear. 


# If you encounter any problems during install, or there is something that doesn't work, please open a new issue with photos.
