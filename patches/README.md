## Xbox Kernel Patches (kpatch - XboxHD+)

| BIOS                                  | Patch Version | Status    | IPS Patch | Guide |
| ------------------------------------- | ------------- | --------- | --------- | ----- |
| m8plus                                |       kp1.0.0 | Stable    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |


### Verified BIOS Hashes
The IPS patch provided should work on all m8plus releases (expect for the forced 480p patched variants). Below is a list of verified BIOS images with their MD5 sum before patching that have been tested and verified.

| BIOS (Filename)                       | MD5 Checksum                     | Status    |
| ------------------------------------- | -------------------------------- | --------- |
| m8plus                                | dfc6288f6b67fd021e1970491c64c0a0 | Verified  |
| m8plus (1.6)                          | 58b8782501983725f984499620ca342b | Verified  |
| m8plus (M8_16_LBA48_IGR_C-06.bin)     | fc9c5dab107a234863714d6452a6d3bb | Verified  |
| m8plus (M8_16_LBA48_IGR_Q-06.bin)     | 0c7ff9e58c7ae9ee5225944ce01daae1 | Verified  |
| m8plus (M8_LBA48_IGR_C-06.bin)        | c5ea8592b48a2bb6b3c288cf263ed9f3 | Verified  |
| m8plus (M8_LBA48_IGR_Q-06.bin)        | 0fc0392198205849849b08f7fd5759c1 | Verified  |
| evox.m8plus.fc.137.bin                | f0decbde3df48a9ecae87336e2a7cbdd | Verified  |

---

## Xbox Kernel Patches (Legacy - XboxHDMI)

| BIOS                                  | MD5 Checksum                     | Patch Version | Status      | IPS Patch | Guide |
| ------------------------------------- | -------------------------------- | ------------- | ----------- | --------- | ----- |
| m8plus                                | dfc6288f6b67fd021e1970491c64c0a0 |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (1.6)                          | 58b8782501983725f984499620ca342b |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_16_LBA48_IGR_C-06.bin)     | fc9c5dab107a234863714d6452a6d3bb |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_16_LBA48_IGR_Q-06.bin)     | 0c7ff9e58c7ae9ee5225944ce01daae1 |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_LBA48_IGR_C-06.bin)        | c5ea8592b48a2bb6b3c288cf263ed9f3 |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| m8plus (M8_LBA48_IGR_Q-06.bin)        | 0fc0392198205849849b08f7fd5759c1 |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| evox.m8plus.fc.137.bin                | f0decbde3df48a9ecae87336e2a7cbdd |         1.4.3 | Verified    | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/m8plus.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20m8plus.md)  |
| iND (iND-BiOS.5003.06.bin)            | b0c482ca1a76a4550c73a391171b8bb1 |         1.4.3 | Beta *      | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/ind-bios.5003.xx.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20ind.md)  |
| iND (iND-BiOS.5003.67.bin)            | ae7bf411d05c3ef1132b97627c65a62f |         1.4.3 | Beta *      | [Link](https://github.com/MakeMHz/xbox-hd-plus/raw/master/patches/ips/ind-bios.5003.xx.ips) | [Link](https://github.com/MakeMHz/xbox-hd-plus/blob/master/manual/Kernel%20Patch%20-%20ind.md)  |


**It is recommended to preform the inital installation and verification using a patch m8plus BIOS.**

## Changelog

### 1.4.x
1.4.x adds preliminary support for upscaling. This should be the last minor update before 2.x.x that adds full support for the new XboxHD features.

### 1.4.3
  *  Clean up visual artifacts introduced in 1.4.2 when using IGR.

### 1.4.2
  *  Initial release.

### 1.4.1
  *  Internal release.

### 1.3.x
1.3.x is a rewrite of the kernel patch with the goal of adding 1.6 support and making the patch more portable. (Requires update of xbox-hd-plus-app for detection)
  *  Added support for 1.6 revision Xbox motherboard
  *  Fixes ALL issues related to non-playable games related to 1.6 compatibility issues! No game patching required. This includes games previously unplayable via any other means, including stock and modified 1.6 systems. (XboxHD+ install required)
  *  Increased compatibility for when the XboxHD+ board is not installed. (Useful for when verifying BIOS is patched pre-installation.)
  *  Send additional data to the XboxHD+ board for edge case handling. (Per-game/title ID handling)

#### 1.3.2
  *  Fix kernel patch not sending correct encoder id. (Fixes colorspace on 1.6 consoles)
