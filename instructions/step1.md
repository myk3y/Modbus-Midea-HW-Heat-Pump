**Step 1: Connect the EW11 to the Midea Heat Pump**

- Power the unit off at the mains connector
- Remove the right-hand cover (as seen when facing the control panel) from the heat pump unit on top of the water tank
- Remove the two screws holding the power connectors to the housing
- Remove all the mounting screws holding the top casing to the main tank
- Carefully feed the power terminal-holding casing through the main top casing and remove the top casing, allowing you full access to the interior
- In the heatpump body, locate the MODBUS cables, AC 220V connectors.

The MODBUS cables are black (MODBUS A), gray (MODBUS B) and yellow (GND)
The connections for the EW11 are:

![Alt text](/images/Elfin%20EW11%20Connection%20Diagram.png)

MODBUS Yellow cable (GND) shares the screw block with 12VDC black/negative wire

![Alt text](/images/Screw%20Block%20Wiring.png)

Mount the transformer and the RS485 module securely to the heat pump. For this I used 3M VHB mounting tape. This 3M product is strong, flexible, but able to be removed if necessary. I have had units mounted over a dozen years and the bond is as strong today as the day I installed it. It will bond to almost any clean surface.

https://www.3mnz.co.nz/3M/en_NZ/vhb-tapes-nz/

Be sure to mount the RS485 module in a way that you can orient the antenna in the same plane as your AP/WiFi router - in other words, if your router has its antenna vertically, make the RS485 antenna vertical too - it will ensure the best connection. The unit is inside a metal casing, surrounded by electronics which can interfere with the signal.

- Once the device is connected and securely mounted, you can power the heat pump back up and connect to the RS485 module

[**Step 2: Connect the Module to WiFi**](instructions/step2.md)

