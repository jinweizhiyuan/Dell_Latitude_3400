# Dell_Latitude_3400
Dell Latitude 3400 Hackintosh OpenCore EFI

|              |                                     |
| ------------ | ----------------------------------- |
| **CPU**      | Core i7-8565U                       |
| **GPU**      | UHD 620 &  NVIDA Geforce MX 130 2GB |
| **RAM**      | 8GB 2666MHz                         |
| **HDD**      | 1TB ST                              |
| **Display**  | 1366 x 768 14' 京东方               |
| **Wifi**     | Atheros Qualcomm Atheroa QCA9377    |
| **Ethernet** | RTL8168/8111/8112                   |
| **Audio**    | Realtek ALC236 (layout-id=3)        |
| **Input**    | PS2 Keyboard & TrackPad             |

## Woking

-  CPU power management.
-  Graphics acceleration.
-  Battery read-out.
-  PS2 Keyboard & trackpad with all macOS gestures.
-  USB ports.
-  Card Reader.
-  HDMI and DP(USB-C) video & audio output.
-  Ethernet.
-  Audio (Internal speakers, 3.5mm headphone jack).
-  Internal microphone.

Not Working:

- I2c HID
-  Wi-Fi
- Bluetooth
-  AirDrop & Handoff.
- 720p WebCam.

## SMBIOS

You will need to generate your own SMBIOS and configure, since is required to fully work with macOS. As per this [guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#platforminfo) you can use the following SMBIOS: MacbookPro 14,1.

Use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate your own unique SMBIOS and then copy each parametter following path (recomended to follow the guide above):

- Config.plist -> PlatformInfo -> Generic
