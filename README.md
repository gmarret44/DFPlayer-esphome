# DFPlayer-esphome
This is the esphome configuration for running a mini dfplayer and playing music on an esp8266/esp32, with home assistant.

Let's start step by step.

First, you need to prepare a micro SD card with a specific hierarchy.

It must be formatted in FAT32.

It must contain an “mp3” folder at the root, containing mp3 files numbered as follows:

0001.mp3

0002.mp3

0003.mp3

etc...

Next, prepare the electronic assembly. (see the diagram file)

Connect the GND and VCC (5V) to the ESP. 

Connect the DFPlayer's RX pin to the ESP's TX pin using a 1k ohm resistor.

Connect the DFPlayer's TX pin to the ESP's RX pin.

Connect speaker + to SPK_1.

Connect speaker - to SPK_2.

Finally, flash the ESP with the esphome-file.yaml file above.

