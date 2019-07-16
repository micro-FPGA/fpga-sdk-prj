Initial port of SCR1 to Cyclone C10LP Refkit

https://shop.trenz-electronic.de/de/TEI0009-02-055-8CA-Cyclone-10-LP-RefKit-10CL055-Development-Board-32-MByte-SDRAM-16-MByte-Flash


Status: UART works (115200), LED's work, Reset button works, not tested: SDRAM, push button

Design was ported from de10lite by changing number of switches and LED's and removing 7 Segment LED's

Note:
there is no new object file, de10lite hex file works, and mini monitor starts 

JTAG debug is included but the pins are assigned to random pins in random PMOD

TODO: 

Reverse engineer the pinmapping of 

https://store.iar.com/product/ADA-MIPI20-RISCV12

And assign JTAG to proper pins and test JTAG debug
