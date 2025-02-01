# Modbus-Midea-HW-Heat-Pump
Integrate the Midea/Chromagen Hot Water Heat Pump with Home Assistant

This is based on the work by **BrittonA** in documenting the MODBUS protocol for the Midea controller  https://gist.github.com/BrittonA/339d25efb934bdb4f451ba7e2f920ba3

And on the work done by **ill_hey** in adapting it for the Elfin-EW11 https://community.home-assistant.io/t/chromagen-midea-170l-heat-pump-hot-water-system-modbus-integration-success/773718

**Background**:

The Midea Heat Pump Hot Water heater is an efficient water heater using heat-pump technology. It comes with an integrated WiFi adapter and associated iOS/Android app, but no easy way of integrating that with Home Assistant.


![Alt text](/images/Midea%20HP300.jpeg)



For the investment of around US$20, you can get full sensor monitoring and control in Home Assistant through the unit's built-in MODBUS protocol and a WiFi-enabled RS485 Serial Server.

There are many such devices, but I have used the Elfin-EW11 for ease-of-use, packaging and price.

[**Installation Instructions**](instructions/Instructions.md)
