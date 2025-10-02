# Windows 11 and Apps Install Notes
The following Windows 11 install notes are set of instructions to expedite and lock-down W11 install. 
It is maintained and updated for general use only. 
The apps available through winget are updated by their respective developers.


### Getting Started
**Follow the Microsoft guidelines on how to create USB ISO image**

See [Microsoft W11 Download](https://www.microsoft.com/en-us/software-download/windows11)

**Windows 11 Operating System install:**

```
1. plug the usb from the MSFT media creation (license maybe required)
2. need network/internet during the latter part of W11 install, best wired ethernet to avoid driver install
3. make sure bios is setup for W11 install if required (see UEFI)
4. shift + f10 and type: start ms-cxh:localonly (this bypasses internet login)
5. w11 install should complete from hereon, unplug usb installer
6. update w11 if needed
```

**Windows 11 Driver, BIOS, and peripherals install:**

```
7. install any necessary bios or hardware drivers (see manufacturer of motherboard)
8. install any necessary drivers or software for peripherals: wireless devices, dac, keyboard, mouse, printers
```

**Windows 11 Apps install:**

```
9. install apps using winget, see link below
```

See [winget-install-apps repo](https://github.com/divemarkus/winget-install-apps)


**Windows 11 bloat removal:**

```
10. clean-up the bloat with crapfixer or do it on your own
11. use openrgb or signalrgb to control all rgb, instead of using manufacturer (see winget script)
```

See [crapfixer repo](https://github.com/builtbybel/CrapFixer)


**Windows 11 security features (DoT):**

```
12. dns over tls or DoT is now available on w11, use it along with your favorite recursive dns providers
```

See [dns over tls script repo](https://github.com/divemarkus/scripts/blob/main/Configure-DoT.ps1)


### Post install
* Make sure you use USB device or NAS to backup all your files. 
* If you don't have any hardware to backup files, use Google Drive.

### winget usage

```
# Misc optional apps
winget upgrade --id Microsoft.VisualStudioCode --exact


# Uninstall by name (best match)
winget uninstall “7-Zip”

# Force-yes on prompts
winget uninstall --id VLC.VLC --silent --accept-package-agreements
```

### Requirements
* .NET Framework 4.0
* PowerShell 5.0+

### More information
Check it out...


