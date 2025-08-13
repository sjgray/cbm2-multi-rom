CBM-II Multi-ROM Adapter
=======================

This is an adapter for CBM-II machines. All ROM sockets including the character ROM will
take an 8K 2364 Masked ROM. 2364 ROMs are also used in other CBM products produced around
the same time. This adapter contains a PLCC socket that can hold a W27C020 EEPROM of 256K.
These EEPROMS are still available and very inexpensive so it doesn't matter if you don't
fill it up. It can erased and re-programmed over and over if needed.

You can have  up to 32 different sets of firmware/characters that are selectable
via DIP Switch with 5 switches. 

To create ROM sets you can use a utility such as my MRB - Multi-ROM Builder which will let
you drag-and-drop and arranges however you like, then build a binary image that can be
written to the EEPROM. I used a TL-866 programmer along with a 32-pin PLCC to DIP adapter
to program the W27C010.


BOM
===

As 5-switch DIP SWITCH versions are not as common you can also install a 6-switch if you
have one. You can also install any lesser number switch if you don't need all 32 slots.
If you only need one slot you can leave off the switch entirely as the resistor-pack will
keep the lines grounded automatically. Finally, you could wire up individual SPST switches
and mount them remotely.

The design uses a 5-pin resistor pack (4 resistors) to be able to fit between the DIP pins.
You need to install a separate resistor for the 5th switch.

You should use round machined-pin headers so as not to damage the sockets on the CBM-II
motherboard.

Gerbers
=======

Gerbers are available in the \gerbers folder. You can simply send the ZIP file to your
favorite pcb manufacturer. I generally use JLCPCB and have had no quality issues with them.


History
=======

* V1.0 created 2025-06-03. Tested and working as expected.

