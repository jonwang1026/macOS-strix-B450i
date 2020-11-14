# macOS-strix-B450i

Hackintosh EFI with OPENCORE 0.6.3 
I have used it on: Catalina 10.15.4 - Catalina 10.15.7 
HAVE NOT USED ON BIGSUR!!

IMPORTANT IF YOU ARE USING THE MY EFI FOLDER
    You will need to create your own SMBIOS if you want to use iMessage, Facetime, any iServices, etc.
    You will also need to create your own USBMAPPING if you encounter any conflicts with your USB ports
    SMBIOS guide
    https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#misc
    USB port mapping guide
    https://dortania.github.io/OpenCore-Post-Install/usb/manual/manual.html#usb-mapping-the-manual-way
    
My current specs
    CPU : AMD Ryzen 7 3700X 3.6 GHz 8-Core Processor
    Memory : Team T-FORCE VULCAN Z 16 GB (2 x 8 GB) DDR4-3200 CL16 Memory
    Motherboard : Asus ROG Strix B450-I Gaming Mini ITX AM4 Motherboard
    Case : NZXT H1 (comes with PSU and 140mm AIO)
    Storage : Western Digital SN550 NVMe 500 GB M.2-2280 NVME Solid State Drive
    Video Card : Gigabyte Radeon RX 5500 XT 8 GB GAMING OC
    Wireless Card: BCM94360NG
        NOTE: I have used a Apple supported wireless card, and it works out of the box.
              Had to replace the onboard one, but there are video
              
BIOS Settings
    Under Boot Settings
        Fast Boot → Disabled
        CSM → Launch CSM → Disabled
        Secure Boot → OS Type → Windows UEFI
        
    Under Advanced Settings
        USB Configuration → XHCI Hand-off → Enabled
        Core Performance Boost → Disabled
        
        
ISSUES YOU MAY FACE
    SLEEP and SLEEP FROM WAKE:
        Pretty much a known issues with AMD builds. No fixes for me, so any insight would be amazing
        
    Discord:
        Pretty much unuseable. Had to use it during a hackathon meeting, and was horrible :(
        FIX can be found here, but have not tested it
        https://discord.com/channels/249992304503291905/263798638373896203/717912500498333746
        
    Random google chrome freezing
        I'm not sure if its my 5500xt that's defective or if its a whatevergreen problem, but my google chrome would freeze 
        for a full second randomly throughout my time of use.
        
PLEASE USE MY CONFIG.PLIST AND EFI FOLDER AT YOUR OWN RISK!!!
    They worked for me, but may not work for your. Please refer to the full guide below before using

Please refer to the dorantia guide for further questions.
    https://dortania.github.io/OpenCore-Install-Guide/
If you need technical help you can use their discord channel via amd osx (also donate if you can)
    https://discord.com/invite/EfCYAJW
