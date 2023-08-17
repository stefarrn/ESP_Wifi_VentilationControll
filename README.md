# ESP_Wifi_VentilationControll
UPDATE:
after assembling the first prototype and making it work, I have applied all necessary changes to the designs and V2.0 should work straight away

![20220614_170043](https://github.com/stefarrn/ESP_Wifi_VentilationControll/assets/80580541/4f2377e1-1869-436b-977b-5588890b1e19)

modification Board in order to controll older ventilation systems over Wifi.

required tools:
1. soldering iron and solder
2. hotplate. heatgun or reflow oven for soldering the surface mount components
3. solder paste and tweezers for soldering surface mount components (ordering a stencil together with the PCBs is highly recommended)
5. computer with USB cable and USB to FTDI adapter or frog pin programmer for the ESP8266
6. Phone or tablet cabaple of running the Arduino IoT remote app
7. some prototyping cables for programming
8. multimeter or oscilocope for troubleshooting

HOW TO USE:
1. order all required parts aswell as the PCB
2. assemble the PCB acording to the schematic (make sure the buck converter is set to around 4-5 Volts before powerup)
3. flash the ESP8266 module over the Pinheader with the help of a USB to FTDI adapter (if you flashed your module before installing it this step can be skipped)
4. solder all the buttons onto pads A1 to D2, where 1 corresponds to the positive and 2 to the negative of the button
5. solder powersupply cables to the VCC and GND pads on the PCB
6. download the Arduino IoT remote app onto your device and log in with the account your ESP is connecting to (this can be done with multiple devices such that everyone can use the ventilation controller)
7. once all this is done and working you can leanback and enjoy :)

OPTIONAL:
1. if your ventilation system uses an LED to indicate wheter it is turned on or off, the pin of said LED that changes potential relative to ground can be soldered ont the LED1 pad for feedback (you might need to change the values for on and off in the software)
2. you can of course also modify the code and UI to your needs

Credits:
ESP8266 schematic symbol, footprint and 3d model by J.Dunmire 
(though I slightly modified the silkscreen on the footprint as iw was overlapping the pads)
buck converter schematic symbol, and footprint were done by me, 3d model by Wilfredo B. de los Reyes I (downloaded from grabcad.com)
schematic and PCB design by me
