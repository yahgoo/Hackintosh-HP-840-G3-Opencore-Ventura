# Hackintosh HP 840 G3 Opencore Ventura
* Opencore EFI for HP 840 G3 running Ventura

## Changes
22092022
- Installed MacOS Ventura 13.0
- Updated to OC 0.8.5 and latest kexts like WEG to spoof SkyLake (SKL) to KabyLake (KBL)
- AltStore 1.5.1 and iPadOS 16.0 works

## Working
- Full graphics acceleration on Intel HD620 iGPU, including brightness control (F5 and F6)
- Multi-display with DisplayPort OOB, VGA 
- Audio, microphone input and headset output (F8 and F9) - Mute button not working
- GigEthernet LAN connection
- Wireless and bluetooth with any compatible card (a DW1560 in my case, no Whitelisting)
left and right USB ports including USB Type-C
- Integrated webcam (OOB)
- CPU power management
- Sleep (Lid, Energy Saver settings, Apple menu, PWR button) & wake (Lid, PWR button)
- Battery management
- Keyboard and touchpad
- Keyboard backlight (F5/F6)
- Touchpad including tap-to-click, scrolling, mouse buttons (can be disable with prt scr key)

![Screenshot](https://github.com/yahgoo/Hackintosh-HP-840-G3-Opencore-Ventura/blob/main/img/macOS%20Ventura%20w%20Apple%20Watch%20Ultra%201600x900.png)

## Set bios settings as follows:
Advanced tab:  
Boot options:  
- Fast Boot = Disabled
- Network (PXE) Boot = Disabled  
Secure Boot Configuration:
- "Legacy Support Enable and Secure Boot Disable"  
System Options:  
- Virtualization Technology (VTx) = Disabled (recommended, Enable also worked)
- Virtualization Technology for Direct I/O (VTd) = Disabled (recommended, Enable also worked)  
Built-In Device Options:  
- Wake On LAN = Disabled
- Video memory size = 64 MB
- LAN/WLAN Auto Switching = Disabled
- Fingerprint Device = Disabled  
Power Management Options:  
- Extended Idle Power States = Disabled
- Deep sleep = You can keep this enabled
- Wake when Lid is Opened = Enabled
- Wake on USB = Disabled

## Credits 
OSXLatitude - Herve, Jake Lo  
EliteMacx86 - EliteMacx86  
Opencore Dev Team  

