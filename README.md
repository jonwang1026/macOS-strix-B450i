# macOS-strix-B450i
![](ignore/desktop.png)
## This EFI is for Opencore 0.6.3
    May not work with newer versions of opencore!!

## Worked on:
    -Catalina 10.15.4 → Catalina 10.15.7 
    
    -HAVE NOT USED ON BIGSUR!!

# !!IMPORTANT!! If you are using this EFI folder:
    -You will need to create your own SMBIOS if you want to use iMessage, Facetime, any iServices, etc. 
        (you can youtube this)
    
    -You will also need to create your own USBMAPPING if you encounter any conflicts with your USB ports
        (you can also youtube this, it will be a lot easier to visually see what they're doing)
        
    -I am using a 5000 series card, so I have adpg=pikera in my BootArgs. If you are using last gen cards take this out. 
    
    SMBIOS guide
    https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#misc
    USB port mapping guide
    https://dortania.github.io/OpenCore-Post-Install/usb/manual/manual.html#usb-mapping-the-manual-way
    
## My current specs
    * CPU : AMD Ryzen 7 3700X 3.6 GHz 8-Core Processor
    
    * Memory : Team T-FORCE VULCAN Z 16 GB (2 x 8 GB) DDR4-3200 CL16 Memory
    
    * Motherboard : Asus ROG Strix B450-I Gaming Mini ITX AM4 Motherboard
    
    * Case : NZXT H1 (comes with PSU and 140mm AIO)
    
    * Storage : Western Digital SN550 NVMe 500 GB M.2-2280 NVME Solid State Drive (MacOS)
    
    * Storage : Western Digital SN750 NVMe 1 TB M.2-2280 NVME Solid State Drive (Windows)
        NOTE: I did dual boot this, so my Windows on this drive is installed as an UEFI
    
    * Video Card : Gigabyte Radeon RX 5500 XT 8 GB GAMING OC
    
    * Wireless Card: BCM94360NG
        NOTE: This is the wifi card that I used to replace the one that came with the board. 
              Bluetooth, wifi, and Airpods all work with this card out of the box.
              
## BIOS Settings
    Under Boot Settings
        * Fast Boot → Disabled
        * CSM → Launch CSM → Disabled
        * Secure Boot → OS Type → Windows UEFI
        
    Under Advanced Settings
        * USB Configuration → XHCI Hand-off → Enabled
        * Core Performance Boost → Disabled
        
    Under EasyMode (Press F7)
        * Turn on "Asus Optimial"
        * XMP Enabled → Profile 1
        
        
## ISSUES YOU MAY FACE
    * SLEEP and SLEEP FROM WAKE:
        Pretty much a known issues with AMD builds. I did do my own USBMapping, and seems to be working on 0.6.3
        
    * Discord:
        Pretty much unuseable. Had to use it during a hackathon meeting, and was horrible :(
        FIX can be found here, but have not tested it
        https://discord.com/channels/249992304503291905/263798638373896203/717912500498333746
        
    * Random google chrome freezes
        I'm not sure if its my 5500xt that's defective or if its a whatevergreen problem, but my google chrome would freeze 
        for a full second randomly throughout my time of use.
        
    * Mouse stuttering issues
        Fixed by downloading steelseries exact mouse. (direct download link below)
            https://downloads.steelseriescdn.com/drivers/tools/steelseries-exactmouse-tool.dmg
        Heard you can also fix this by adding this line into the terminal, but not sure.
            "defaults write .GlobalPreferences com.apple.mouse.scaling -1"
        
# PLEASE USE MY CONFIG.PLIST AND EFI FOLDER AT YOUR OWN RISK!!!
    They worked for me, but may not work for you. Please refer to the full guide below before using. 
    I will not be reponsible for any damages to your computer.
## Dortania Guide
    An amazing guide: https://dortania.github.io/OpenCore-Install-Guide/
    
## If you need technical help you can use their discord channel (and donate to amdosx if you can)
    Discord: https://discord.com/invite/EfCYAJW
    
    Donation to Amd OSX: https://forum.amd-osx.com/index.php?dbtech-donate/drives/amd-os-x.1/donate
    
    
    

If you read all the way here olive you, and don't worry theres a lot of people who are here to help :)

