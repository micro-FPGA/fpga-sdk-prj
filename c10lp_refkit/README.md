Initial port of SCR1 to Cyclone C10LP Refkit

https://shop.trenz-electronic.de/de/TEI0009-02-055-8CA-Cyclone-10-LP-RefKit-10CL055-Development-Board-32-MByte-SDRAM-16-MByte-Flash


Status: UART works (115200), LED's work, SDRAM works (may need check params!), Reset button works, not tested: push buttons

Design was ported from de10lite by changing number of switches and LED's and removing 7 Segment LED's

Note:
there is no new object file, de10lite hex file works, and mini monitor starts 

JTAG debug is included but the pins are assigned to random pins in random PMOD

TODO JTAG pin assign: 

https://store.iar.com/product/ADA-MIPI20-RISCV12

| #|##|Signal|Net|Pad|
|--|--|--|--|--|
| 1| 1|TDO  |P6_IO1|B19|
| 2| 7|TDI  |P6_IO5|A18|
| 3| 2|nTRST|P6_IO2|A19|
| 4| 8|TMS  |P6_IO6|B18|
| 5| 3|TCK  |P6_IO3|B20|
| 6| 9|nRST |P6_IO7|A17|
| 7| 4|-    |
| 8|10|-    |
| 9| 5|GND  |
|10|11|GND  |
|11| 6|VREF |
|12|12|VREF |




