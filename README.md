# OC-AMD-Ryzen-9-7900X-ASUS-TUF-X670E-RX6800XT-AQC107
Hackintosh Opencore V 0.9.7 Sonoma 14.2.1
## Specification
|  Component  | Model  |
| ------------ | ------------ |
| CPU  | AMD Ryzen 9 7900X |
| Motherboard | ASUS TUF Gaming X670E-PLUS Wifi  |
| RAM  | 64GB (2x32GB) Corsair Vengeance DDR5-6400 DIMM2 and DIMM4 |
|  GPU  | Dell Radeon RX 6800 XT 16GB in 1st 16x slot (@16x) |
| Ethernet1  | Realtek RTL8125  O/B |
| Ethernet2  | TP-Link TX401 (AQC107) in 2nd 16x slot (@4x) |
| MacOS Drive  | Corsair MP600 Pro LPX 2TB in M2_3 slot (@4x) |
| Windows 11 Drive  | Corsair MP600 Pro XT 1TB in M2_1 slot (@4x) |
| BIOS  | v2214 + iGPU Disabled in BIOS Settings |
| USBMAP  | Including the ports required to control Aura |


## ACPI
- SSDT-CPUR.aml
- DSDT-X670E-TUF-WIFI-patched.aml
- SSDT-EC-USBX.aml
- SSDT-SBUS-MCHC-AMD.aml

## Kext
- Lilu
- VirtualSMC
- LucyRTL8125Ethernet
- WhateverGreen
- AppleMCEReporterDisabler
- AMDRyzenCPUPowerManagement
- AppleALC
- RestrictEvents
- USBToolBox
- UTBMap
- RadeonSensor
- SMCRadeonGPU
- SMCAMDProcessor
- USBToolBox
- UTBMap
- NVMeFix
- AMFIPass

## Not Working
- M2 Wifi 6: MT7921K is not supported (Enabled in Windows)

### MacOS version : Sonoma (14.2.1)
### SMBIOS : MacPro7.1
### Motherboard Bios version : 2214
### Based on https://github.com/kakabala/ryzentosh-AMD-Ryzen-9-7900X-TUF-X670E
