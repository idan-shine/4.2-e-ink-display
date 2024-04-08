# 4.2-e-ink-display
Conf and fonts for a e-ink displayed based on esphome for displaying temp and other info
Don't forget adding: "template: !include forecasts.yaml" to your configuration.yaml file

Based heavily on makai's project published here: https://community.home-assistant.io/t/air-quality-sensors-e-ink-display-using-esphome/201776

Because I am not using a DIY AQI sensor but rater a Aqara temp+TVOC sensor I changed it a bit, also my house is smaller, so I preferred a rooms view and not a floor one. 
Finally, I wanted a different forecast section, so, first release was this:

![PXL_20230701_085006713](https://github.com/idan-shine/4.2-e-ink-display/assets/101454370/f294bb7a-d7bc-4138-902e-82754922a138)

(AQI/TVOC is not showing here. its in the empty space in the middle, I still waited for the sensor to arrive at that point)

But at the end I had to rotate the screen because of the space I had on the wall. Because I liked all the original aspect rotation, I just changed rotating from 270 to 0,
redistributed a few things (like time, date and forecast) that didn't fit in anymore, switch temps and humidity positions and fine tuned a bit.

# finished product looks like this:

![WhatsApp Image 2023-07-15 at 15 04 28](https://github.com/idan-shine/4.2-e-ink-display/assets/101454370/a2f5919e-22a6-4b64-9af1-a051a0e8655d)

(Still need to fix the wall where the AC line is coming in, also the lighting isn't very good at the moment of shutting the pic)

- The days of the week for the forecast as well of the forecast are coming from openwheatermap integration
- the TVOC is read by an Aqara TVOC sensor in the living room like this one (that where I took my design idea's from for the e-ink screen):

![zigbee-air-quality-sensor-aqara-tvoc-](https://github.com/idan-shine/4.2-e-ink-display/assets/101454370/67cfb3b3-223b-4d93-b463-b5e7e2242496)

- additional two sensors (Sonoff and ubiquiti) are providing data from the bedroom and outside.
- frame if DIYed from red oak, very nice (and strong) material I decently recommend!

Enjoy!
