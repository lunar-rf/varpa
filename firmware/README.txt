Dependencies
------------

gcc-avr binutils-avr gdb-avr avr-libc avrdude make git

To install all dependencies, run:
make deps

Fuse Settings
-------------

Fuse settings are defined in the Makefile as follows:

LFUSE = 0xFF
HFUSE = 0xD9
EFUSE = 0xFF
LOCK = 0xFF

System Reset
------------

To exclusively execute a soft reset, run:
make reset

Firmware Compilation
--------------------

To exclusively build the firmware, run:
make build

Firmware Flash
--------------

To exclusively execute a firmware flash, run:
make flash

Usage
-----

Only two commands are required to build and flash
the firmware onto the ATmega328P.

Simply run:
make

Then run:
make upload

Note:

If you encounter issues performing a soft reset, use:
make force-upload

