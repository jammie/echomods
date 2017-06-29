## Alternative to Tobo


### Brief

* Need to get 200ns wide square pulses, both in the positive and negative.
* Control of pulses must be through 3.3 or 5V tolerant logic
* pulses height must be selectable (say with a jumper?) for ~20V, 40V, 80V (for positive pulses) and -20, -40V, and -80V for negative.
* Only power supply available is 5V



See this [application note](http://ww1.microchip.com/downloads/en/AppNotes/AN-H53.pdf) - recommend MD1213 and TC6320 


High voltage source: https://datasheets.maximintegrated.com/en/ds/MAX5025-MAX5028.pdf (3 -> 30V) to be used with a [555 DC-DC convertor](http://www.eleccircuit.com/the-many-dc-to-dc-converters-using-ic-555/)

Signal back from the diod is to be clipped by [MD0100](http://ww1.microchip.com/downloads/en/DeviceDoc/MD0100.pdf) + back to back diods. Design should be such as MD0100 and diods are easily removable (maybe through a very small add-on PCB) in case they burn.

### Power use:

The pulser sends with a 500us repeat, 10mA at 5V. So power may not be an issue here.