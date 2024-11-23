### Intel-i3-12100F-RX6600XT-SOYO-B660M-EFI

**macOS**: Ventura 13.7
**OpenCore**: 1.0.2 with dualboot

#### Specifications
|Item|Description|
|-|:-------:|
|CPU|Intel Core i3 12100F|
|Motherboard|Gigabyte B660M GAMING AC DDR4|
|Memory|Crucial 32GB DDR4 3600Mhz (16GBx2)|
|SSD1|Intel® SSD 760p Series 512G / macOS Ventura 13.7|
|SSD2|SK hynix PC801 1TB / Windows11 23H2|
|GPU|Sapphire AMD Radeon RX6600 XT 8G|
|Wi-Fi / Bluetooth|BCM94360CS2 + NGFF adapter (PCIex1 slot)|

#### BIOS Version F28
#### BIOS Configuration

`Load Optimized Default` first then save and restart and go to BIOS again.

### Tweaker:
* Extreme Memory Profile: **Profile 1**
* Advanced CPU Settings:
  - Hyper-Threading Technology: **Enabled**
  - Intel Turbo Boost Technology: **Auto** (not the 3.0 one)

- Advanced Memory Setting:
    - Memory Enhancement Setting: **Enhanced Performance**

- Advanced Voltage Settings > CPU/VRM Settings:
    - CPU Vcore Loadline Calibration: Low

### Settings:

* Platform Power:
  - ErP: **Disable**
  - Power Loading: **Enabled**
  
* IO Ports:
  - Initial Display Output: **PCIe 1 Slot**
  - Above 4G Decoding: **Enabled**
  - Above 4G MMIO BIOS assignment: **Disabled** (Will cause the issue with 2nd sleep)
  - Super IO Configuration → Serial Port: **Disabled** (Will cause the issue with Apple Watch unlock)

  - USB Configuration:
    - XHCI Hand-off → **Enabled**
    - Legacy USB Support → **Enabled**
    - USB Mass Storage Driver Support → **Enabled**
    - Port 60/64 Emulation → **Disabled**

  - Network Stack Configuration → Network Stack: **Disabled**
  
* Miscellaneous:
  - Intel Platform Trust Technology(PTT) → **Enabled**
  - Vt-d → **Enabled**

### Boot: 
  - CFG Lock: **Disabled**
  - Fast Boot: **Disable Link**
  - Windows 10 Features: **Windows 10**
  - CSM Support: **Disabled**
  - Secure Boot: **Disabled** (Secure Boot will be disabled by default, but good to check)

---------------------

##### OFF
- Onboard CNVi Module Control-Disable Integrated
- Intel VT-D ？
- Speed Select Technology
- CFG LOCK
- Fast BOOT
- Secure Boot
- Serial/COM Port
- Parallel Port
- Compatibility Support Module (CSM).
- Intel SGX
- Intel Platform Trust
- CAM (Clever Access Memory, AKA Resize Bar) 

##### ON
- Re-Size BAR Support
- SR-IOV Support
- Err Ready
- VT-x ？
- Execute Disable Bit
- SATA Mode: AHCI

VT-d ？ / XMP2.0 ？

#### REMEMBER generate and replace with your own SMBIOS infos

![screenshot](https://raw.githubusercontent.com/suxiaogang/Intel-i3-12100F-B660M-RX6600XT-EFI/refs/heads/main/images/macOS%2013.7.jpg)