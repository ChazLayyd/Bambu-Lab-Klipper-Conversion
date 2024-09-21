# Bambu Lab Klipper Conversion!

Welcome to my page! The goal of this project is to have a **fully non-destructive** upgrade path to [Klipper](https://www.klipper3d.org/), on a Bambu Lab P1S. This means replacing the existing electronics with open-source hardware. My project right now is in the works, but should be fully working hopefully soon. Stick around for updates.

# Updates as of 21/09/2024 22:49PM GMT+1

Upon further inspection the SSR appears to be reusable, I need to probe the pins with my multimeter to find the controlling pins in their PicoBlade connector. Then I can wire those up to the new control board for controlling the AC bed.

Bed thermistor is confirmed as a NTC 100kΩ 3950. Can be configured as Generic 3950 in klipper config. Shows accurate temperature readings from my old bed, which I removed and added my own JST connector onto.

The piezo sensors appear to be reusable in some way, just need to figure out the wiring to them and then configure them as needed in klipper.

I have designed a quick PCB from JLCPCB that can convert the stock PicoBlade connectors of the Chamber Exhaust fan, and Aux Cooling fan, to be easily converted to a JST connector. Just plug and play. Will test if it works once those arrive, these are ridding of the PWM control sadly, so I am unsure if they even work. Atleast not at their true full power. But I will test their functionality as soon as they arrive.
