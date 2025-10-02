# Windows 11 and Apps Install Notes
The following Windows 11 install notes are set of instructions to expedite and lock-down W11 install. 
It is maintained and updated for general use only. 
The apps available through winget are updated by their respective developers.


### Getting Started
**Follow the Microsoft guidelines on how to create USB ISO image**

See [Microsoft W11 Download](https://www.microsoft.com/en-us/software-download/windows11)

**Windows 11 Operating System install:**

```
# plug the usb from the MSFT media creation (license maybe required)
# need network/internet during the latter part of W11 install, best wired ethernet to avoid driver install
# make sure bios is setup for W11 install if required (see UEFI)
# bypasses microsoft account login and use local only
(shift + f10)
# type:
start ms-cxh:localonly
# press enter and it will go through a boot process to create local account
# install should complete from hereon, unplug usb installer
# update w11 if needed
```


**Windows 11 Driver, BIOS, and peripherals install:**

```
# install any necessary hardware drivers/bios (see manufacturer of motherboard)
# install any necessary drivers/softwares for peripherals: wireless devices, dac, keyboard, mouse, printers
```



**Windows 11 Apps install:**

```
# install apps using winget instead of doing it manually (link below)
```

See [winget-install-apps repo](https://github.com/divemarkus/winget-install-apps)



**Windows 11 bloat removal:**

```
# clean-up the bloat with crapfixer or do it on your own
# use openrgb or signalrgb to control all rgb, instead of using manufacturer (see winget script)
```

See [crapfixer repo](https://github.com/builtbybel/CrapFixer)



**Windows 11 security features (DoT):**

```
# dns over tls or DoT is now available on w11, use it along with your favorite recursive dns providers
```

See [dns over tls script repo](https://github.com/divemarkus/scripts/blob/main/Configure-DoT.ps1)



**Windows 11 additional tools or apps (optional):**

```
# if you have nvidia/amd gpu (graphics card), install the apps related to your gpu manufacturer
# enable hdr from windows 11: System > Display > HDR 'on'
# if using nvidia gpu 30 series or higher, enable rtx vsr and hdr from gpu app
# for playing videos or movies use vlc version 3.0.19. this version strictly supports vsr/hdr:
https://downloads.videolan.org/testing/vlc-rtx-upscaler/
# rtx vsr and hdr will also upscale youtube videos
# enable spatial sound from windows 11: System > Sound > (choose the sound device/output) > Spatial sound: Windows Sonic for Headphones
```



**Windows 11 threat hunting (optional):**

```
# use the following osquery scripts below to hunt down threats or malicious apps
```

See [osquery script repo](https://github.com/divemarkus/osquery/blob/main/W11-Threat-Hunting-v1)



### Post install
* Use USB device or NAS to backup all your files. Use Google Drive for remote backups 
* Schedule to update all your apps with winget



### Requirements
* .NET Framework 4.0
* PowerShell 5.0+

### More information
Check it out...


