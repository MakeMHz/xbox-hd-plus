# Kernel Patch - ind.5003.xx

### DO NOT FLASH TO TSOP! YOU HAVE BEEN WARNED!

Start by placing the IPS patch inside of an empty folder with the ind.5003.xx BIOS.

![Step 1](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_1.png)

Open XBtool, choose 'Multi' for BIOS Type, and click ‘Unpack’, then choose your BIOS for the system you’re patching.

![Step 2](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_2.png)

![Step 3](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_3.png)

At this point, you should have an xboxkrnl.img file inside subfolder of the BIOS location.

![Step 4](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_4.png)
![Step 4](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_4b.png)

Now open up Lunar IPS and click ‘Apply Patch’

![Step 5](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_5.png)

Choose the ind-bios.5003.xx.ips patch file.

![Step 6](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_6.png)

Set 'Files of type:' from 'Most Common ROM Files' to 'All Files' and choose the xboxkrnl.img

![Step 7](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_7.png)

![Step 8](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_8.png)

Now open back up XBtool, choose 'Multi' for BIOS Type, and click 'Pack'. Choose the patched xboxkrnl.img

![Step 9](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_9.png)

For the 'Save As' give the new BIOS a unique name, such as ind-bios.5003.06.(HD1.4.3), and click save.

![Step 11](https://github.com/MakeMHz/xbox-hd-plus/raw/master/manual/images/patch/ind_patch_10.png)

Your BIOS is now patched! Flash the BIOS to your modchip of choice and verify by launching the XboxHD+ app.
