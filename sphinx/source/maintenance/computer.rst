Computer
========

.. contents::
   :backlinks: top
   :local:

Computer Boot Procedure Outside of Vehicle
------------------------------------------

1. Check that the mother board is set to 12V mode. See\: http://store.enochsystems.com/resources/techdocs/2014/MX87QD_Manual_V1.0.pdf#page=36
2. Attach power cord (frayed ends to molex connector) to binding post terminals on Power Supply

   a. Use Channel 1 & Channel 2 in parallel

3. Plug in Power Supply
4. Set supply to CV (Constant Voltage)

   a. Turn current dial until the indicator LED nearby lights up green. This indicates that it is in CV mode.

5. Set supply Voltage to 12.0V
6. Connect power cord to mother board.
7. Computer should boot.

   a. To launch GUI: `sudo service lightdm start`
