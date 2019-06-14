# Adafruit-NeoPixel-8x8-Matrix 

__Format is EagleCAD schematic and board layout__

<a href="http://www.adafruit.com/products/1487"><img src="assets/image.jpg?raw=true" width="500px"><br/>Click here to purchase one from the Adafruit shop</a>

Put on your sunglasses before wiring up this LED matrix - 64 eye-blistering RGB LEDs adorn the NeoMatrix for a blast of configurable color. Arranged in an 8x8 matrix, each pixel is individually addressable. Only one microcontroller pin is required to control all the LEDs, and you get 24 bit color for each LED.

Wiring it up is easy: there are two 3-pin connection ports. Solder wires to the input port and provide 5VDC to the +5V and ground pins, then connect the DIN pin to your microcontroller. If you're using our NeoPixel Arduino library, use digital #6. You'll also need to make a common ground from the 5V power supply to the microcontroller/Arduino. Since each LED can draw as much as 60mA (thats up to 3.5 Amps per panel if all LEDs are on bright white!) we suggest our 5V 2A power supply. For most uses, you'll see about 1-2A of current per panel.

If, say, you need MORE blinky, you can chain these together. For the second shield, connect the DIN connection to the first panel's DOUT. Also connect a ground pin together and power with 5V. There you go! You can chain as many as you'd like although after 4 or more panels you may run low on RAM if you're using an UNO. Watch your power usage too, you may need a 5V 10A power supply for so many of these!

There is a single data line with a very timing-specific protocol. Since the protocol is very sensitive to timing, it requires a real-time microconroller such as an AVR, Arduino, PIC, mbed, etc. It cannot be used with a Linux-based microcomputer or interpreted microcontroller such as the netduino or Basic Stamp. Our wonderfully-written Neopixel library for Arduino supports these pixels! As it requires hand-tuned assembly it is only for AVR cores but others may have ported this chip driver code so please google around. An 8MHz or faster processor is required.

[Our detailed NeoPixel Uberguide has everything you need to use NeoPixels in any shape and size. Including ready-to-go library & example code for the Arduino UNO/Duemilanove/Diecimila, Flora/Micro/Leonardo, Trinket/Gemma, Arduino Due & Arduino Mega/ADK (all versions)](http://learn.adafruit.com/adafruit-neopixel-uberguide)

## License

Adafruit invests time and resources providing this open source design, 
please support Adafruit and open-source hardware by purchasing 
products from Adafruit!

Designed by Adafruit Industries.  
Creative Commons Attribution, Share-Alike license, check license.txt for more information
All text above must be included in any redistribution
