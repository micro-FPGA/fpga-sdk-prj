Initial port of SCR1 to Cyclone C10LP Refkit

https://shop.trenz-electronic.de/de/TEI0009-02-055-8CA-Cyclone-10-LP-RefKit-10CL055-Development-Board-32-MByte-SDRAM-16-MByte-Flash


Note: there is no new object file, de10lite hex file works, and mini monitor starts UART baudrate 115200

JTAG is mapped to P6 PMOD (the left most one close to usb connector) pinoput for this adapter:

https://store.iar.com/product/ADA-MIPI20-RISCV12

Note: nTRST pin on this adapter goes to unpopulated 2mm pin header holes only so it would not have contact to PMOD pin.

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

Debug test status: 
* Segger J-Link OK
* IAR I-Jet OK
* Open OCD - not tested

Note: for IAR TCK should be set to 1MHz



