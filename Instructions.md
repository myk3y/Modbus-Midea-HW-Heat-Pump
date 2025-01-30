**INSTRUCTIONS**:

Purchase an RS485 to WiFi module. There are many available - in board form, as a packaged module, as a DIN unit for mounting on a rail. 

The module I used is the Elfin EW11 RS486 WiFi Serial Server from Hi-Flying.com. http://www.hi-flying.com/elfin-ew10-elfin-ew11

![Alt text](images/Elfin-EW11%20RS485%20Serial%20Server.png)

I sourced my unit from Aliexpress, with supporting antenna, connector cables and mounting block: https://www.aliexpress.com/item/1005006252294801.html but this unit is available from many vendors.


**Overview**:

The basic procedure is: to connect the module to power, to configure it to use your local WiFi AP, to set the operating parameters on the EW11, to connect it to the Midea MODBUS, to configure Home Assistant to poll the device and to check the results in Home Assistant.

To power the EW11, I used an AM11-12W12C 220V AC to 12V DC transformer. It has an output of 1000mW - more than enough to drive the EW11. Again, I sourced this component from Aliexpress, but any number of modules would do the same job: https://www.aliexpress.com/item/1005005937263063.html

![Alt text](images/)

**Step 1: Connect the EW11 to the Midea Heat Pump**

- Power the unit off at the mains connector
- Remove the right-hand cover (as seen when facing the control panel) from the heat pump unit on top of the water tank
- Inside the cover, locate the MODBUS cables, AC 220V connectors.

The MODBUS cables are black (MODBUS A), gray (MODBUS B) and yellow (GND)
The connections for the EW11 are:

![Alt text](images/Elfin%20EW11%20Connections.png)

Configure the WaveShare module. In mode, you need to set Modbus TCP <=> Modbus RTU. The default username and password is admin admin

Connect the WaveShare module to your Midea 170L heat pump. The cables are Yellow = GND, Gray = B, Black = A.

Using File Editor in Home Assistant navigator to your configuration.yaml file and add this line 

modbus: !include modbus.yaml

Using File Editor, create a modbus.yaml file and copy the configuration above.

Adjust the host to match the IP address of your WaveShare module.
