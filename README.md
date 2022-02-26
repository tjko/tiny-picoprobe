# tiny-picoprobe
Tiny PicoProbe PCB, when you want to use PicoProbe to debug your [Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/) programs without a breadboard...

![Tiny PicoProbe PCB](images/tiny-picoprobe.png)

Designed with [KiCad](https://www.kicad.org/) 6.0.  PCB allows mounting Pico directly or using headers:

![Assembled Tiny PicoProbe](images/assembled.jpg)
![Tiny PicoProbe with headers](images/headers.jpg)

## Kerbers
Kerber files ready to be sent to a PCB maker (like JLCPCB, etc):
* [PCB Version 1.0](kerbers/tiny-picoprobe-v1.zip)

## Assembly
PCB contains footprints for a 0805 size SMD LED and resistor to provide power indicator. Power indicator is optional.

ID|Type|Description|Mouser P/N|LCSC P/N
--|----|-----------|----------|---------
D1|LED (0805)|Pad is suitable for handsoldering 0805 size LEDs, 0603 should work as well...|710-150080GS75000 (?)|C434432
R1|7.5k (0805)|Depending on LED used choose appropriate resistor. Green high-intensity 0805 LEDs typically work nicely with resistor in 5k to 10k range|603-RC0805FR-077K5L|C229003

Note, if soldering Pico directly on the PCB, then 1" diameter shrink tubing can be used to wrap the pico and PCB in nice insulated package.

## Credits
Idea for this PCB came from [Fabien-Chouteau/picoprobe-pcb](https://github.com/Fabien-Chouteau/picoprobe-pcb) (check his version as he sells it on Tindie).

KiCad Pico model/footprint that was used can be found here [ncarandini/KiCad-RP-Pico](https://github.com/ncarandini/KiCad-RP-Pico)
