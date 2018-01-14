Solito PCB
==========

BOM
---

```
Item: 			MCU, ATMEGA32A-AU 
Farnell Part:		1704563 
Cost:			£3.24
Package:		TQFP-44 
Notes:			3.3V max speed is 10MHz, also in 44-QFN package (too small for hand solder?),
Notes:			http://www.wormfood.net/avrbaudcalc.ph

Item:			Power supply: NCP1117ST33T3G 3.3V, 1A, 20V max, 3.5V minimum input
Farnell Part:		1652366RL 
Cost:			£0.41
Package:		SOT-223
Notes:			See page 8 of data sheet for thermal pad size

Item:			Power supply capactiors (10uF)
Farnell Part:		9697012RL
Cost:			£0.11 each
Package:		5.4mm high, radial can, SMD
Notes:			Need 2 per regulator, input should be 20V capable

Item:			Crystal: SMD HC-49S  9C-7.3728MAAJ-T 7.3728 Mhz
Farnell Part:		1842344 
Cost:			£0.38
Package:		HC49/US
Notes:			Choose 9.216MHz Xtal, or 7.3728 Mhz for a bit more UART speed (230400)
Notes:			9.216MHz is a rare part and out of stock.

Item:			Crystal for RTC 32.768kHz
Farnell Part:		2101352 
Cost:			£0.71
Package:		Unknown, 4.9 x 1.8mm
Notes:			RTC, capacitance 12.5pF, guard ring the x-tal as in the Dallas DS

Item:			15pF SMD capactitor for crystal, MC0805N150J500CT 
Farnell Part:		759193 
Cost:			£0.018 for 10 
Package:		0805
Notes:			12-22pF ok, see AtMega DS p26, we need 2

Item:			RTC DS1307, DS1307ZN+ (N+ is low temp, but is cheapest)
Farnell Part:		9725253 
Cost:			£3.61
Package:		SOIC8
Notes:			Requires 4.5V minimum
Notes:			p7. Datasheet, requires crystal, 32.768kHz, 45kOhm max res, 12.5pF typical capac.
Notes:			Requires li-ion coin cell , 48mAh lasts 10 years, optional, ground VBat if not used
Notes:			DS1338 is 3.3V alt.

Item:			RTC DS1338
Farnell Part:		1379714
Cost:			£3.22
Package:		SOIC8
Notes:			Like DS1307 but 3.3V, needs 12.5pF crystal 32.768kHz

Item:			Coin cell holder, CH291-1220LF
Farnell Part:		2064722
Cost:			£0.52
Package:		Specifc
Notes:			CR1220 battery, cheap, SMD mount, super caps off uAh in SMD sizes. 4.7mAh / year

Item:			GREEN SMD LED
Farnell Part:		8529906 
Cost:			£0.40 for 10
Package:		0805 (1.25 x 1.3mm)
Notes:			20mA max

Item:			BLUE SMD LED
Farnell Part:		1686076RL 
Cost:			£0.38 for 10
Package:		0805 (1.25 x 1.3mm)
Notes:			20mA max

Item:			2.54mm pitch pin
Notes:			0.025" pitch square wire -> 0.64mm

Item:			BC817-40 NPN PWM transistor for LED
Farnell Part:		1081225
Cost:			£0.20 for 10
Package:		SOT23
Notes:
```
