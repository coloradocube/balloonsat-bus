# Version 0.1

Consider what we have designed and gotten manufactured as of 2022-04-20 to be Version 0.1.

# Version 0.2

The following is a list of modifications to do per board for Version 0.2 to be ordered on Monday, 2022-04-25. All of these will be converted to issues. Also, **the boards will be split up into separate repositories**.

## Sensors
1. The PIC programmer pins:
   1. Should be at 90 degrees toward the outside.
   2. Their ends should be [supporting rail width] mm in from the edge of the board.
   3. Their height (from board to 90-deg bend) has to be either 5.32 mm or 3.19 mm. These are the 
   4. Their depth (horizontal part after the 90-deg bend) should be sufficient for the femail connector of the PIC programmer (~ 6 mm).
   5. There should not be any other components in the way of the PIC programmer on both sides of the pins for a total width of 39.72 mm.
2. The LEDs should be in a row along the edge [supporting rail width] mm in.
3. Button switch should be closer to the edge [supporting rail width] mm in.
4. There needs to be an I2C connection for an externally-hanging (outside of the craft shell) thermal sensor. The sensor housing should also be designed.
5. (Nice to have) An IMU sensor integrated into the I2C-to-CAN design paradigm of the sensor board.

## CDH
1. Should be re-programmable in place, w/o disassembling the stack. _Moving the CM 4 (currently the only one) between the CDH and the IO Board will eventually damage the connector._
2. The two UART connectors have to be pushed in toward the center of the board or turned sideways.

## EPS
1. Same as (1) for [sensors](#sensors).
2. The redesign by [abrannigan](https://github.com/orgs/coloradocube/people/ajbrannigan) to fix the 5V issue.

## Battery pack
1. The connector to the EPS should be pushed in toward the middle of the board so that it is away from the edge of the board.
2. Silkscreen "+" and "-" for each battery position. I know the holders have them, but white on green is easier to get right at launch when it might be dark.

## Miscellaneous
1. The combined height of the bottom-board backplane connector and the mid-board backplane connector (plastic parts, when flush against both boards) is perfect to let the PIC programmer in. The height/thickness of PIC connector is 10.87 mm.
