### Hackintosh-Intel-i3-12100F-B660M-RX580-EFI

**macOS**: Ventura 14.7.1
**OpenCore**: 1.0.2 with dualboot

#### Specifications
|Item|Description|
|-|:-------:|
|CPU|Intel Core i3-12100F|
|Motherboard|Gigabyte B660M GAMING AC DDR4|
|Memory|Crucial 32GB DDR4 3600Mhz (16GBx2)|
|SSD1|SK hynix PC801 1TB / Windows11_LTSC2024_24H2|
|SSD2|Dahua C900 PLUS M.2 2280 NVMe 512GB SSD / macOS_Ventura_14.7.1|
|GPU|AMD Radeon RX 580 8G|
|Wi-Fi / Bluetooth|BCM94360CS2 + NGFF adapter (PCIex1 slot)|

#### BIOS Version F28
#### BIOS Configuration

`Load Optimized Default` first then save and restart and go to BIOS again.

### Tweaker:
* Advanced CPU Settings:
  - Hyper-Threading Technology: **Enabled**
  - Intel Turbo Boost Technology: **Auto**

### Settings:

* Platform Power:
  - ErP: **Disable**
  - Power Loading: **Enabled**
  
* IO Ports:
  - Initial Display Output: **PCIe 1 Slot**
  - Above 4G Decoding: **Enabled**
  - Above 4G MMIO BIOS assignment: **Disabled**
  - Super IO Configuration → Serial Port: **Disabled**

  - USB Configuration:
    - XHCI Hand-off → **Enabled**
    - Legacy USB Support → **Enabled**
    - USB Mass Storage Driver Support → **Enabled**
    - Port 60/64 Emulation → **Disabled**

  - Network Stack Configuration → Network Stack: **Disabled**
  
* Miscellaneous:
  - Intel Platform Trust Technology(PTT) → **Enabled**
  - Vt-d → **Disabled**

### Boot: 
  - CFG Lock: **Disabled**
  - Fast Boot: **Disable Link**
  - Windows 10 Features: **Windows 10**
  - CSM Support: **Disabled** (it depends, if your graphic card is too old and does not support UEFI boot, you should enable CSM)
  - Secure Boot: **Disabled**

### OTHER: 
  - LEDs in System Power On State: **On**
  - Mouse Speed: **4 X**


#### REMEMBER generate and replace with your own SMBIOS infos
#### [Fixing Broadcom Wi-Fi on macOS 14 Sonoma](https://github.com/perez987/Broadcom-wifi-back-on-macOS-Sonoma-with-OCLP)
#### [Fixing Shutdown/Restart](https://dortania.github.io/OpenCore-Post-Install/usb/misc/shutdown.html#fixing-shutdown-restart)

![screenshot](https://raw.githubusercontent.com/suxiaogang/Hackintosh-Intel-i3-12100F-B660M-RX580-EFI/refs/heads/main/images/MacPro.png)
![screenshot](https://raw.githubusercontent.com/suxiaogang/Hackintosh-Intel-i3-12100F-B660M-RX580-EFI/refs/heads/main/images/HardwareAcceleration.jpg)