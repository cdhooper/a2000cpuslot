Amiga 2000 CPU slot adapters

rev1_pcb contains Gerbers for the minimal 68000 slot adapter.
rev1_90_pcb contains Gerbers for a 68000 slot adapter where the 68000 socket
is rotated by 90 degrees. This may allow some accelerators to be installed
in the system which otherwise would not fit.

----------------------------------

Be sure to solder the 100nF capacitor on the rear of the PCB if you
are installing a 68000 CPU. This will improve stability.

For the general case of installing a CPU in the slot, you will want
to remove the 68000 CPU from the motherboard. It's possible that you
can have the card disable the onboard CPU by setting a jumper between
the BOSS pin and GND. You will want to remove the ECLK jumper in that
case. Otherwise, if there is no 68000 installed in the motherboard,
be sure to add a jumper on the ECLK header.

You should not need to add solder blobs on the FC0, FC1, or FC2 pads
or add diodes on the CPU IPL0, IPL1, or IPL2 pins.
