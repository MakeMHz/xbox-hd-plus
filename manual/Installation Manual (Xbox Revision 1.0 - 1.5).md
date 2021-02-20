# XboxHDMI Installation Guide
### Xbox Revision 1.0 -1.5

- [Brief Overview](#brief-overview)
- [Preperation](#preperation)
  * [Kit Contents](#kit-contents)
  * [Wire Prep](#wire-prep)
  * [XboxHDMI Board Prep](#xboxhdmi-board-prep)
- [Step 1 - Motherboard Prep](#step-1---motherboard-prep)
- [Step 2 - Jumper Wires](#step-2---jumper-wires)
- [Step 3 - Flex Installation](#step-3---flex-installation)
- [Step 4 - Aux Wires](#step-4---aux-wires)
- [Step 5 - Wrapping Up](#step-5---wrapping-up)

### Brief Overview
For a Brief Overview, Please visit the YouTube video below.

![Image of XboxHDMI YouTube Video](images/YouTube.png)
<p align="center">https://bit.ly/339G98T</p>

### Preperation
Before your adventure begins, it's imperative to ensure that you have a fully working, tested, and modified xbox. (The current version of the BIOS patch requires a HDTV AV/component cable to test)

Please thoroughly test your system before attempting to install the XboxHDMI kit.
This guide also assumes that you watched the installation video linked above.

This guide is for Xbox motherboard revisions 1.0 - 1.5 with a Conexant or Focus encoder.
**<p align="center">Apply the kernel patches and verify it's activated by running the XboxHDMI application on the Xbox before teardown, as this will fix certain kernel bugs in some games!</p>**
<p align="center">https://github.com/MakeMHz/xbox-hdmi/blob/master/patches/README.md</p>

### Kit Contents
Check your kit for missing or damaged pieces before moving forwards.

- XboxHDMI Main Board
- XboxHDMI Flex PCB
- 26AWG Stranded Red Wire for the 5V and 1.8V connections.
- 26AWG Stranded Orange Wire for the SPDIF connection.
- 26AWG Stranded Black Wire for the ground connections.
- 22AWG paired Wire for the SMBus connection.
- 3D printed board spacer
- 3D printed HDMI port cover
- 2 replacement screws

### Wire Prep
It's imperative to cut each wire as close as possible to our recommendations, but not shorter. if additional wire is needed then make sure to use wire of similar quality and gauge.

After cutting each wire, strip each side of the wires. It's recommended for the cleanest install to strip about 2mm from one side (for the connections to the Xbox motherboard) and about 3mm on the other side (for connections to the XboxHDMI board). Make sure to twist the stranded wires and pre-tin each one.

**Cut List and Lengths (end to end, before stripping)**

<table>
  <tr>
    <th>Black Wire</th>
    <td>25mm</td>
    <td>GND 2 Connections Near the SDA/SCL pads</td>
  </tr>
  <tr>
    <th>Black Wire</th>
    <td>28mm</td>
    <td>GND 1 Connection Near the SPDIF pad</td>
  </tr>
  <tr>
    <th>Red Wire</th>
    <td>35mm</td>
    <td>1.8V Connection</td>
  </tr>
  <tr>
    <th>Red Wire</th>
    <td>48mm</td>
    <td>5V Connection</td>
  </tr>
  <tr>
    <th>Orange Wire</th>
    <td>45mm</td>
    <td>SPDIF Connection</td>
  </tr>
  <tr>
    <th>Paired Wire</th>
    <td>90mm</td>
    <td>SMBus Connection</td>
  </tr>
</table>

### XboxHDMI Board Prep
Begin by adding solder to all of the connection pads (GND, SDA, SCL, SPDIF, 1V8, 5V). This is important as there's little room once everything is installed.

### Step 0 - QSB Installation
Xbox revisions 1.0 and 1.1 (Single row power supply connector and Conexant encoder) requires the installation of a QSB board. Follow the [Installation Manual QSB](Installation%20Manual%20QSB.md) first before continuing. (If you received a kit without the QSB and need one then contact support@makemhz.com or purchase one from [MakeMHz.com](https://makemhz.com))

### Step 1 - Motherboard Prep
The first step is to remove the motherboard from the Xbox. There are plenty of guides on the internet on how to do so and won't be repeated here as it's pretty straight-forward.

It's recommended that you remove the GPU heatsink since there's very little room between it and where the flex cable will be installed. We've found that the best approach is to apply very low heat to the heatsink, around 100°C / 212°F, while applying very light force twisting to the heatsink.

**It's very important not to force the heatsink off by attempting to pull it straight up as this could damage the GPU.** *(There's at least one person who's managed to do this in the past, unrelated to the project, and even though it's very unlikely, it's noted here to let others know to be careful!)*

The thermal compound on the GPU can be cleaned off with a basic solvent such as Arctic Silver Arcticlean Thermal Cooling Material Remover or with WD-40. When re-applying the heatsink, make sure to add **ample** PC thermal paste. *(in this case, more is better as a bit too much should not effect thermals and is ultimately safer as the GPU does not have an embedded thermal sensor for overheating protection).*

After this, you can remove the AV port. Please refer to the installation video for more information on the different ways to accomplish this.

And finally, make sure to clean the area where the flex will be installed with IPA.

![Image of XboxHDMI YouTube Video](images/Step1.png)
<p align="center"><i><b>Note that removing the CPU heatsink is not required.</b></i></p>

### Step 2 - Jumper Wires
This step gets its own section as it's very easy to forget, and can be a pain if forgotten since the pins are located on the bottom of the board.

We need to make two connections on the bottom of where the AV port used to be, so that the Xbox thinks that an HD AV cable is plugged in. Use a scrap piece of wire to make these connections.

![Image of AVIP Connections](images/Step2-AVIP-Connections.png)
![Image of AVIP Connections](images/Step2-Pinout.png)

### Step 3 - Flex Installation
This section will be mostly screenshots of the Xbox video encoder and where the flex connects. Pay close attention to the alignment of the flex cable and **take your time while installing!**

After the flex is installed, the Xbox should still be bootable.

#### Best Practices
- Pre-tin both sides of the flex by applying ample flux and running solder across each pad before soldering to the Xbox motherboard.
- Pre-shape the flex. Gently shape the flex so it's close to the final shape before soldering. The flex must lay flat and properly aligned when installed.
- Take your time!

**Completed Install**

![Image of Flex Installed](images/Step3-Flex-Installed.png)

**Overview View**

![Image of Flex Board Layout](images/Step3-Flex-Overview.png)

**Right Connections**

![Image of Flex Board Layout](images/Step3-Right.png)

**Left Connections**

![Image of Flex Board Layout](images/Step3-Left.png)

**Bottom Connections**

![Image of Flex Board Layout](images/Step3-Bottom.png)

### Step 4 - Aux Wires
Start with connecting each of the pre-cut wires. The wires for 5V and SPDIF should lay flat across the motherboard running towards the right.

#### Ferrite Bead Removal
Next to the Video encoder is a ferrite bead, labeled FB3B1, that needs to be removed. this can be easily done by heating it up with a soldering iron and a bit of solder.

![Image of Ferrite Bead Removed](images/Step4-FB-Removed.png)

#### AV Port/Encoder Connections
Connect each of the pre-cut wires according to the wire cut chart above. the wires for 5V and SPDIF should lay flat across the motherboard running to the right.

![Image of Wire connections](images/Step4-Wire-Connections.png)

#### SMBus Connections (SDA and SCL)
Using the paired wire connect one wire to each side of the PIC16.

![Image of SMBus Connections](images/Step4-PIC16.png)

### Step 5 - Wrapping Up

#### 3D Printed HDMI Panel
Insert the 3D printed HDMI part in between the metal shielding and the Xbox case.

![Image of 3D printed HDMI Panel](images/Step5-3DHDMI.png)

#### 3D Printed Spacer
Place the spacer as shown below in black.

![Image of 3D printed Spacer](images/Step5-Spacer.png)

<p align="center"><b><i>I forgot to take a photo for the manual... MSPaint works though.</b></i></p>

### Re-install the Xbox Motherboard
Place the Xbox motherboard back into the case. Make sure to screw the motherboard back in. There's one screw located under where the XboxHDMI will be installed.

### Install the XboxHDMI Board
Place the XboxHDMI board in the system and screw it down with the two provided screws.

Connect each wire to their corresponding pads on the XboxHDMI board.

Carefully connec the flex cable to the FPC connector. Be very careful. it may take a couple of tries as sometimes the flex will want to go in at an angle. if this happens, then pull it out and gently push it back in. ***Do not force it in. Make sure the flex is not inserted at an angle!***

![Image of XboxHDMI Installed](images/Step5-Finished.png)
<p align="center"><i><b>This is a photo of a test system. Ignore the missing parts of the case...</b></i></p>
