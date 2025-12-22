# RooK Mk3.1

RooK is a retro gaming console based on the Raspberry PI CM4/CM5. It has all the peripherials you need to be used as an old (modernish) console:

* HDMI for audio and video out.
* Barrel jack for 5V power input, because we love the simplicity of barrel jacks.
* an audio jack for, well... speakers!
* 4 USB ports for up to 4 modern gamepads.
* A cartridge slot!
* 3 Buttons to shut RooK down, exit the game and restart the game.

## How it all works

It's quite simple: instead of having an onboard SD card, the SD cards are installed onto separate PCBs for the cartridges. Once you put a cartridge in, RooK powers up and boots off the SD card in the cartridge.

Of course, unwrapping the SD cards can be tedious, so we built a cartridge reader.

It works out of the box with retropie, except for the three buttons. In this repository you find the software needed to enable those buttons. It's best done immediately after installing retropie, before you customize your setup.

## In this repository

There are 3 folders:

* software contains the sources for the .deb file to easily install overwatch and it's configuration. You'll find the .dep file in there as well, if you don't want to build it yourself. The source is compressed, as we have to ensure ownership and file privileges. Something git tends to ignore ;)
* PCBs contains all the designs for the PCBs involved: 
    * Cartridge - the PCB for cartridges
    * CartridgeReader - should be self-explanatory
    * KeyswitchCarrier - holds the switches for the three keys
    * Mainboard - the biggest of them.
    * Parts and CM4-Files are referenced in the aforementioned design files
* STLs contain the STL files for the case and the cartridge. You'll find our FreeCAD designs in there as well.

## I wanna build one!

Well for now, you have to produce and order the parts yourself. We're working on this. Stay tuned and keep an eye out at [rook.computer](https://rook.computer).

There is a building guide in the wiki.
