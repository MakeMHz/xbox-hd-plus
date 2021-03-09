## Xbox Kernel Patches

| BIOS                                  | MD5 Checksum                     | Patch Version | Status      | IPS Patch | Guide |
| ------------------------------------- | -------------------------------- | ------------- | ----------- | --------- | ----- |
| m8plus                                | dfc6288f6b67fd021e1970491c64c0a0 |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (1.6)                          | 58b8782501983725f984499620ca342b |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_16_LBA48_IGR_C-06.bin)     | fc9c5dab107a234863714d6452a6d3bb |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_16_LBA48_IGR_Q-06.bin)     | 0c7ff9e58c7ae9ee5225944ce01daae1 |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_LBA48_IGR_C-06.bin)        | c5ea8592b48a2bb6b3c288cf263ed9f3 |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_LBA48_IGR_Q-06.bin)        | 0fc0392198205849849b08f7fd5759c1 |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| evox.m8plus.fc.137.bin                | f0decbde3df48a9ecae87336e2a7cbdd |         1.3.1 | Verified    | [Link](https://github.com/MakeMHz/xbox-hdmi/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hdmi/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |

## Changelog

### 1.3.x
1.3.x is a rewrite of the kernel patch with the goal of adding 1.6 support and making the patch more portable. (Requires update of xbox-hdmi-app for detection)
  *  Added support for 1.6 revision Xbox motherboard
  *  Fixes ALL issues related to non-playable games related to 1.6 compatibility issues! No game patching required. This includes games previously unplayable via any other means, including stock and modified 1.6 systems. (XboxHDMI install required)
  *  Increased compatibility for when the XboxHDMI board is not installed. (Useful for when verifying BIOS is patched pre-installation.)
  *  Send additional data to the XboxHDMI board for edge case handling. (Per-game/title ID handling)
