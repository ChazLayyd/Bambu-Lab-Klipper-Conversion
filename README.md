# Bambu Lab Klipper Conversion!

Welcome to my page! The goal of this project is to have a **fully non-destructive** upgrade path to [Klipper](https://www.klipper3d.org/), on a Bambu Lab P1S. This means replacing the existing electronics with open-source hardware. My project right now is in the works, but should be fully working hopefully soon. Stick around for updates.

# Update as of 02/11/2024 00:33AM GMT+0

I do apologise to lack of updates here, but I bring AMAZING news! Almost the entire printer is now fully controlled via Klipper! We are talking fans, hotend, and now THE BED! The load cells are the last tackle if I ever want to get around to that, but I am honestly loving the whole microprobe setup, it works perfectly fine.

# Update as of 10/10/2024 11:58PM GMT+1

Hello again! I have made some good progress on the P1S. I have swapped the hardware out with a BTT Manta M5P and CB2, provided for free by BIGTREETECH. I haven't got the heat bed to work yet, but I do have a temperature readout for the thermistor! I have also done a lot of probing around with a multimeter on the piezoelectric amplifier boards and believe that I have found the piezo signal line. I just need to supply it with the necessary power and then we could have working load cells. I am working on the heat bed as soon as I can, just doing some test prints using the old MCU to control the bed temperature. Not ideal at all but it's working.

I am posting more active and random updates on my [Twitter page](https://x.com/chazmakes/)! So I suggest that you follow me over there for more active updates.

# Update as of 24/09/2024 07:28AM GMT+1

A suitable replacement power supply has been found that is a drop in replacement and gives +100w. However the problem with this is that it only accepts 230v input, meaning NA users are out of luck for this route. External may be necessary for this to work in NA. I will continue to try fit a better power supply into the right side of the chamber but this will be hard to do easily. A custom printed rear panel may be needed for this to work.

# Update as of 22/09/2024 07:02AM GMT+1

I have designed a custom PCB that will allow me to control almost everything. It allows use of all the stock fans in the rear minus the MCU cooling fan, as the 92mm chamber fan is going to be reused to cool off all the fancy new electronics more quietly.
It also adds support for dual auxilary cooling, either via adding another standard 120mm blower with a jst connector from the likes of GDStime, or using another official Bambu 120 blower. Be aware of the amperage here, some boards may not be able to handle more than 1A per fan connector. Bambu lab fans run off 0.5 amps, both will be controlled off a single JST XH2.54 connector. Not ideal I know, but thats the route I've chosen for how easy it is.

Will soon be testing out SSR functionality, just need to wait on these new PCB's to arrive which could take a week or two. Hopefully no longer than this.

# Update as of 21/09/2024 22:49PM GMT+1

Upon further inspection the SSR appears to be reusable, I need to probe the pins with my multimeter to find the controlling pins in their PicoBlade connector. Then I can wire those up to the new control board for controlling the AC bed.

Bed thermistor is confirmed as a NTC 100kΩ 3950. Can be configured as Generic 3950 in klipper config. Shows accurate temperature readings from my old bed, which I removed and added my own JST connector onto.

The piezo sensors appear to be reusable in some way, just need to figure out the wiring to them and then configure them as needed in klipper.

~~I have designed a quick PCB from JLCPCB that can convert the stock PicoBlade connectors of the Chamber Exhaust fan, and Aux Cooling fan, to be easily converted to a JST connector. Just plug and play. Will test if it works once those arrive, these are ridding of the PWM control sadly, so I am unsure if they even work. Atleast not at their true full power. But I will test their functionality as soon as they arrive.~~
