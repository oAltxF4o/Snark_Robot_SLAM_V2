Most of the information I have on the L02 PCB comes from my previous work on the revere engineering the L01 PCB.
The header for connecting the the RVC base PCB is the same between both models.

With the exception of the console UART, there are no test pads on the top side of the PCB. 
The console UART test pads are carried through to the bottom side of the PCB with vias.

A curriousity I have yet to figure out is the 7-pin header located at the bottom of the PCB about half way accross. 
The non-power/gnd pads are all used with I2S0 as one of the alt functions, and 4 of 5 of them have are also used for SPI1 alt function.

It is sad to see with this version too that none of the JTAG points have been routed to test pads, not have any of the main emmc lines.
There is a nice change though, The USB_ID pin has been broken out, and routed to a test pad... what does this mean? I don't know yet.

As of right now I have only done the RE of the board to find out what lines I need at the moment, but I will do a full RE in the future with a BOM.
