<br /> <p align="center"><a href="https://github.com/theXappy/MF800-LTE-5G-USB-MODEM" target="_blank"><img src="img/4g_lte.png" width="200"></a></p>

<p align="center"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Intro
I bought this "LTE '5G' USB Dongle WiFi" from AliExpress around 2024.  
After playing with it for a while, I decied to document all the quirks/tricks I've learned.  
SoC seems to be: `Qualcomm Snapdragon 410 (MSM8916)`  
USB Hardware IDs: `VID_05C6 PID_90B6`  
Modem Identifiers (fetched with AT commands):
```
ATI
Manufacturer: QUALCOMM INCORPORATED
Model: 4094
Revision: MF800_V2.0_21_V01R01B05  1  [Sep 07 2015 23:00:00]
SVN: 01
IMEI: +CGSN:860018046000213
+GCAP: +CGSM

AT^SWVER
^SWVER: MF800_V2.0

AT^HWVER
Part=206  version=1.0
```

## Table of Contents
### 🌐 Web App & ADB
1. See [https://github.com/theXappy/UZ801-LTE-USB-MODEM?tab=readme-ov-file#-web-app--adb](UZ801-LTE-USB-MODEM)

### ☎️ Modem
1. See [https://github.com/theXappy/UZ801-LTE-USB-MODEM?tab=readme-ov-file#%EF%B8%8F-modem](UZ801-LTE-USB-MODEM)

### 📱Screen Control
1. See [https://github.com/theXappy/UZ801-LTE-USB-MODEM?tab=readme-ov-file#screen-control](UZ801-LTE-USB-MODEM)

### 🪄 Firmware Backup/Flashing
1. See [https://github.com/theXappy/UZ801-LTE-USB-MODEM?tab=readme-ov-file#-firmware-backupflashing](UZ801-LTE-USB-MODEM)
