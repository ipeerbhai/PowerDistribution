# PowerDistribution
This design is for a small wiring board to provide power to a robotic rover.

It's designed in 3 sections.

## Part 1: High Current ESC Pads ##
This part is 3 thick traces without masking to push high voltage/current power in a short segment.  It is completely unfused, and should be pushed to a smart, power-hungry board like an ODrive.  The lack of masks is to enable solder as a wire for high-current and voltage use cases.

## Part 2: Battery Monitoring ##
This part has 2 SMD resistors in a simple voltage divider circuit.  The resistor values chosen are 22M-ohm (RMCF0805FT22M0) and 1M-ohm(RC0805FR-071ML.  This enables voltage detection on a Teensy 4.1 from 0 to 50V.

## Part 3: Switch and buck converters ##
A large swtich pad for a single pole, single throw switch,
a small pad buck converter for a raspberry pi or other SBC, and 2 large pads for very high-current buck converters for Star-power servos.
For the switch, Amazon part number: B078KBC5VH
For the RPi Buck converter, Amazon part number: B079N9BFZC
For the Star-Power converter, Amazon part number: B0819Y8PJZ
