# Seeed XIAO-ESP32-S3/C3 based DSC Keybus Interface
## Features
- The mcu modules are in wide distribution and available from reliable sources such as Mouser and Digikey.
- A u.fl antenna connector on the mcu for an external antenna when the device is installed in a metalic DSC enclosure
- Mounting holes and form factor compatible with DSC expansion modules
- MOSFET level converters
- Optional NPN driver for the data line when using the device as a diagnostic tool. Using the same GPIO for both reading and writing data makes it impossible to monitor the bus when writing. NPN driver chosed because library inverts output.
- Fixed 5VDC buck DC-DC converter that can be disconnected when powering via USB
- Serial I/O extended to a header for diagnostic output when device is powered by the Keybus
- Pads for soldering modules with castellated pads. This allows for either headers or direct soldering of the mcu and DC-DC converter
- Thru-hole pads to allow assembly with conventional not SMD soldering skills
## Questions for next version
- TVS diodes on clock and data?
- Extend additonal GPIOs to a header?
- Convert serial I/O header to 6 pins for compatibility with FTDI TTL-232R-3V3 cable.
## Precautions
- Don't power the device without an antenna connected. Regardless of its low power output, there are reports that the power amp gets fried. 
## Parts List
- J1 TE_282837-4 1x4 screw terminal
- J2 1x2 2.54mm vertical pin header
- J3 1x3 2.54mm vertical pin header
- Q2,Q3 2N7000 inline
- Q1 2N3904 inline
- U1 Seeed XIAO ESP32S3 with u.fl antenna connector
- U2 MP1848EN 5V DC-DC buck converter
- R1 1K 1/4W resistor
-    u.fl to RP-SMA cable assembly
-    RP-SMA 2.4GHz antenna
-    Reverse locking support Essentra Components RLCBSR-6-01
