# xbox-hdmi

## Getting Started

Please read the manual first

### 1.0 - 1.5 revisions of the Xbox
[Installation Manual](<manual/Installation Manual (Xbox Revision 1.0 - 1.5).md>)

[Quick Solder Board](<manual/Installation Manual QSB.md>)

### 1.6 revision of the Xbox
[Installation Manual](<manual/Installation Manual (Xbox Revision 1.6).md>)

## Essential links

### BIOS patch

Please read [Kernel Patch for M8+](<manual/Kernel Patch - m8plus.md>)

### XBOX HDMI Application

[XBOS HDMI Download Application Download](https://github.com/MakeMHz/xbox-hdmi-app/releases)

### 3D Printed Parts

| Part         | Source (Fusion360)      |
|--------------|-------------------------|
| HDMI Panel   | [https://a360.co/3l2h5Ya](https://a360.co/3l2h5Ya) |
| Board Spacer | [https://a360.co/30kox9a](https://a360.co/30kox9a) |

## Installation FAQs

### What do the blinking lights mean?

#### Green
Signal lock (CLKI), but there could still be an issue with horizontal sync (HSYNC) and or virtical sync (VSYNC).

#### Blue
Status. Blinking is normal.

### What is the best way to debug an issue if I have no video?

It is recommended to visually inspect your work under a microscope or magnifying glass.

USB microscopes are now relatively cheap and compatible with most computers and phones. These inexpensive microscopes will often show as webcams for these systems.

### How good / clean does the soldering need to be?

Very good.

Check for:
- bridged connections
- leftover flux
- connections that may not have enough solder

### How accurate do the lengths of the cables need to be?

Cable length may impact the quality of the signal, so try to use the recommended lengths. Those provide enough wire to make the connection and provide some degree of flexibility in working.

### Can I test the soldering with a multimeter continuity test?

Multimeter continuity tests are not reliable in determining if connections are bridged or if connections are not well connected for this installation, so they are not recommended.

### What do I do if my main board doesn't look the same as the photos?

The board is labeled for each spot. The references show these labels and other boards will have the same labels in similar spots.

There is some expectation that installers have some familiarity with printed circuit boards.

### Does the patched BIOS need to be installed to get video?

Short answer is `no`.

You can get video from a modchip OS such as Xenium OS which loads prior to the patched BIOS.

The console should also load without the patched BIOS.

The BIOS patch is recommended and will add additional features.
