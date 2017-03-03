# Raspberry Pi Zero sized Hat
This a KiCad template for a Raspberry Pi Zero sized Hat. It is based on the 
[Raspberry Pi B+ Hat template](https://github.com/xesscorp/RPi_Hat_Template) from Xess Corp. Xess Corp did all the hard work here.

Currently there is no mechanical definition for Raspberry Pi Zero Hats so the 
[mechanical definition](https://www.raspberrypi.org/documentation/hardware/raspberrypi/mechanical/rpi-zero-v1_2_dimensions.pdf)
for the Raspberry Pi Zero itself was used instead.

The board outline looks like this:

<img src="meta/RPi_Zero_Hat-brd.png" style="width:100%">

## Status
This template has not been used in a design yet so verify before using.

Below is the original README. Folow the instructions below to use this template.

# Raspberry Pi B+ Hat

Expansion Board
----------------------------

This is a project template for a 
[Raspberry Pi B+ Hat](https://github.com/raspberrypi/hats).

This base project includes a PCB edge defined according to 
[this specification](https://github.com/raspberrypi/hats/blob/master/hat-board-mechanical.pdf).
Both a thru-hole and a surface mount connector are provided, along with a different
PCB edge for each. Just keep the PCB edge and connector type that you're using for your design
and delete the others.

The component footprints used in this template are [here](https://github.com/xesscorp/RPi_Hat.pretty).

The board outline looks like this:

<img src="brd.png" style="width:100%">

Using the Template
----------------------------

To use the Raspberry Pi Hat template with the through-hole connector, do the following:

1. Open the schematic. Remove the SMD connector, J1.
2. Generate the schematic netlist.
3. Generate the .cmp file. (The J2 connector will be the only component in it.)
4. Open the PCB. Hover your mouse over the connector and hit **e** to edit it. Select the J1 SMD connector. In the **Move and Place** section of the **Footprint Properties** window, select the **Free** radio button. Then click **OK**. The SMD connector should now be unlocked so it can be removed.
5. Read in the netlist from the schematic. In the **Extra Footprints** section of the **Netlist** dialog window, select the **Delete** radio button. Then click **Read Current Netlist**. The J1 SMD connector should disappear. Then click **Close**.
6. Finally, delete the upper two arcs and the edge of the board outline.

To use the Raspberry Pi Hat template with the SMD connector, do the following:

1. Open the schematic. Remove the through-hole connector, J2.
2. Generate the schematic netlist.
3. Generate the .cmp file. (The J1 connector will be the only component in it.)
4. Open the PCB. Hover your mouse over the connector and hit **e** to edit it. Select the J2 through-hole connector. In the **Move and Place** section of the **Footprint Properties** window, select the **Free** radio button. Then click **OK**. The through-hole connector should now be unlocked so it can be removed.
5. Read in the netlist from the schematic. In the **Extra Footprints** section of the **Netlist** dialog window, select the **Delete** radio button. Then click **Read Current Netlist**. The J2 through-hole connector should disappear. Then click **Close**.
6. Finally, delete the lower two arcs and the edge of the board outline.

(c)2015 XESS Corp.
