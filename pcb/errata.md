Errata
======

Issues found to address in next board revision.

v1.0
----

* The ground pin for the display is weak and delaminates from the board
* MISO pin not required on the display header
* The LED driver overheats with a 10W RGB unit - provide more heatsinking
  for driver
* The rotary encoder lines A and B are reversed. This is bad because the
  indent on the encoder sits on the boundary of a line B change. Therefore
  the encoder is prone to firing many times with very little movement.
* The ground pad for the decoupling cap for the accelerometer needs a
  thermal relief as it's very difficult to solder otherwise
* The mounting holes need to be enlarged in general
* The power connector pads should be more robust
* The battery overlaps with the ADXL345 stabilising hole
* The rotary encoder push button is missing a debounce cap
* Rotary debouncing could be improved? It's currently crude
* The board should support the HC-05 BT module which can operate
  in slave/master
* CS pin on ADXL345 should be tied to VDD to enable I2C
* PB3 is used for the display, but it is OC0 which is useful for
  other things - use a different pin
