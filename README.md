# The Open Source Sync Stripper
A project to strip sync from composite video signals.

So this project is a PCB, that takes a Scart connector,runs the composite video signal through an LM1881 and outputs C-Sync. It then breaks out the RGB and C-Sync signals to an SMA conector, and audio to either a headphone jack or simple pads to solder to.

From the SMA connectors, you can get SMA to BNC cables, and use this for the inputs for an Extron Crosspoint, or any 15khz monitor with BNC RGBS inputs.

You MUST have 5-12V on pin 8 for this to function.

You should be familiar with Surface Mount and Through Hole soldering to assemble this project.

There is no bottom solder mask, which means the audio pads on the bottom are not labeled. The center 2 pads are the two grounds, and the Left pad is the Left channel, and Right pad is the right channel.

It is also possible to use this device as a Scart to BNC adapter without the sync stripping abilities. This is ONLY if you have C-Sync coming out of the composite pin, or don't have a need for C-Sync. 
Situation 1: C-Sync mod. Some people do this if they never want composite again, and get C-Sync internally and run the signal down the composite conductor. 
Situation 2: If you don't have an extron, and will only be using this as a passthrough device, hooked up directly to your B/PVM.

Just bridge pads 1 and 2 on the SOIC8 pads, and short out the pads for C1. This will just passthrough whatever is coming down the composite pin, and output it to the SMA connector.

Otherwise, as of 1/9/2018 I have added a passthrough board entitled "ScartBNCnostrip". This is just a simple passthrough, where pin 20 is tied directly to the "S" sma connector. THe LM1881 and caps/resistors have also been removed in this version.


ALSO! If you're looking to stack them, the Jackpost I used is:

https://www.digikey.com/products/en/hardware-fasteners-accessories/board-spacers-standoffs/582?k=8405k

Digikey PN 36-8405-ND
