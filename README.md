## Bambu Lab Klipper Conversion!

![Klipper Logo](/images/logo_new.png)

## Join the [**Community Discord!**](https://discord.gg/W6B5mBejuC)

## As requested multiple times- you can support the project on [**Ko-Fi**](https://ko-fi.com/chazmakes). It's not necessary, but if you want to help out then all support is greatly appreciated!

> [!Caution]
> This Project is in **BETA**, doing this conversion is fully at your own risk, I am not responsible for any damages done to your machine. This also will likely void your warranty.

Welcome to the Bambu Lab Klipper Conversion page! The project is in beta at the moment. This is a **non-destructive (PCB Only)**, or **destructive** upgrade path to [**Klipper**](https://www.klipper3d.org/), on a Bambu Lab P1 (or X1, untested). This means replacing the existing electronics with open-source hardware. A custom PCB has been designed to make everything plug and play with the fans, heatbed etc. The project runs on a fork of Klipper known as [**Kalico**](https://github.com/KalicoCrew/kalico), previously known as DangerKlipper. Make sure to get yourself familiarized with [**The Official Klipper Docs**](https://www.klipper3d.org/) and [**The Kalico Docs**](https://github.com/KalicoCrew/kalico/tree/main/docs)

You can find the BOM [**here**](https://docs.google.com/spreadsheets/d/187OusyREO98zsinT2Vspcr3hRtGYJvgfUr3D4DhnsbQ/edit?usp=sharing).

You can find the Instructions Guide [**here**](https://docs.google.com/document/d/10jUgWAk6IcKfLQbqBuNKKKB1ifLewu4NGnTodkZCtSU/edit?usp=sharing).

The current release is <ins>**0.1** </ins>

## What works? (as of release <ins>**0.1**</ins>)
- ✓ The full hotend and extruder assembly
- ✓ Heatbed control with the Stock SSR
- ✓ The entire motion system is unchanged
- ✓ All fans work if wired correctly (PWM and Tach control needs to be added)
- ✓ Bambu Lab AMS does work via the [**OpenAMS project**](https://github.com/OpenAMSOrg)

## What doesn't work? (as of release <ins>**0.1**</ins>)
- ✖ Load cell probing (Replaced for now with a Biqu Microprobe), but a custom board is in the works.
- ✖ Webcam (You can purchase the X1C camera and wire it up as a USB camera)
- ✖ Stock display
- ✖ Toolhead boards
- ✖ Filament runout detection
- ✖ Not everything is plug and play. There is a PCB design available to make this non destructive You will need to splice on extension cables + JST XH 2.54 or DuPont 2.54 connectors.

## Why?

At first, this was a joke. More of a "why not" sort of thing. But as time went on, I really started to think of the benefits of putting Klipper on this machine. All my other printers run on Klipper.. so why not make the Bambu also run on Klipper! It provides a great platform for modding, such as adding extra fans, a nicer webcam, maybe some better controlled neopixel lighting, fully custom toolheads.. And most importantly, having the heatbed capable of running at 110C! Whatever you can think of, you can do it with this platform. It also completely eliminates the Bambu Cloud, allowing you to run everything locally, or even use your own cloud service.. Who else loves privacy?!
