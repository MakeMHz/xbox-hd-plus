# Kernel Patch - m8plus

### DO NOT FLASH TO TSOP! YOU HAVE BEEN WARNED!

Start by placing the IPS patch inside of an empty folder with the M8plus BIOS. (The BIOS release pictured below also included a separate BIOS for 1.0-1.5 and another for 1.6)

![Step 1](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_1.png)

Open EVtool and click ‘Unpack’, then choose your BIOS for the system you’re patching. (M8plus.bin for 1.0 - 1.5 systems and M8plus_16.bin for 1.6 systems)

![Step 2](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_2.png)

![Step 3](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_3.png)

At this point, you should have an m8plus_kernel.img file in the same folder has the BIOS.

![Step 4](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_4.png)

Now open up Lunar IPS and click ‘Apply Patch’

![Step 5](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_5.png)

Choose the m8plus.ips patch file. 

![Step 6](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_6.png)

Choose the m8plus_kernel..img

![Step 7](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_7.png)

![Step 8](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_8.png)

Now open back up EVtool and click 'Pack'. Choose the m8plus_kernel.img

![Step 9](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_9.png)

Select the correct BIOS as the Base ROM. (M8plus.bin for 1.0 - 1.5 systems and M8plus_16.bin for 1.6)

![Step 10](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_10.png)

For the 'Save As' give the new BIOS a unquie name, such as M8plus_patched.bin, and click save.

![Step 11](https://github.com/MakeMHz/xbox-hdmi/raw/master/manual/images/patch/m8plus_patch_11.png)

Your BIOS is now patched! Flash the BIOS to your modchip of choice and verify by launching the XboxHDMI app.
