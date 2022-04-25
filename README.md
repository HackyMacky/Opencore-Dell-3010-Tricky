# Opencore-Dell-3010-Tricky
A working Opencore configuration for the Dell Tricky Chromebox. Also tested working for HP CB1 Zako Chromebox (Atheros Wifi card replaced with Intel AC7260).

## DISCLAIMER 
I will not be held responsible for any damage, permanent loss of data or any sorts of consequences that may arise by using my configuration files on your devices. Please use at your own risk.

## Current Release
- Opencore 0.7.9
- Monterey 12.3
- All latest kexts as of March 31, 2022

## Notebook Specifications

| Specification  | Model |  Remark  |
| ------------- | ------------- | ------------- |
| FW  | Mr.Chromebox's CoreBoot | 4.16  |
| CPU  | Intel i7-4600U  |
| iGPU  | Intel HD 4600 | 
| Storage  | Transcend 128GB M.2 SSD  |
| RAM  | 8GB (2x4GB) PC3L |
| Ethernet  | Realtek RTL8111 |
| Wi-Fi  | Intel Wireless AC-7260 (HMW)stock  |
| Bluetooth  | Intel Bluetooth   |
| Audio  | HD4600 + Realtek (layout 1)   |


## What's working
- Mostly everything
- Wi-Fi & Bluetooth, Ethernet
- Display outputs (DP + HDMI)
- Headphone jack, microphone
- USB ports mapping

## What's not working
- Sleep issue (wake triggers a reboot)

## Not tested
- AppleID and iServices

## Quirks/issues
- Sleep issue (wake triggers a reboot)

## Setup Note
1. Ensure to generate your own SMBIOS serial number etc and update the config plist
2. Edit the Realtek kext (info.plist) > fallbackMAC with your own ethernet mac address else ethernet will not work
3. Kindly disable sleep once installed as there seems to be an issue with sleep where waking triggers a reboot

## Credits
- All credits & rights goes to the maintainers, contributors and developers of the Opencore project and respective kernel extensions.
- MrChromebox for the chromebox FW
- Apple Inc.
