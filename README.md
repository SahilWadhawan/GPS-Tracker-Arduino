# GPS-Tracker-Arduino
Parents often worry about their children when they are away from them. Have they safely reached school? Are they alone at home? Or are they at the playground with friends? – these are some of the questions that bothers parents all over the world.

So, I made a smart tracker that can keep track of a child. Besides this, the device can also be used to track your vehicle location and other objects.

# - Specifications -
Arduino GPS tracker with ATGM336H module, SD card module, LiPo battery, and ATSAMD21 microcontroller.

<a id="diagram"></a>
# - Diagram -
Here, we are wiring the ATGM336H GPS module via SPI to the Arduino Xiao (ATSAMD21) board:
![ATGM336H wiring to ATSAMD21](/images/atgm336h_datalogger_wiring.jpg)
![ATGM336H wiring to ATSAMD21 - table](/images/atgm336h_datalogger_wiring_table.jpg)
<a id="arduinocode"></a>
# - Arduino Code -
The Arduino code used to log GPS data is found at:

- [gps_datalogger.ino](/arduino/gps_datalogger.ino)
<a id="python"></a>
# - Python Code -
The Python scripts used to parse the GPS coordinates from the .csv log file and plot them atop a street map can be found at:

- [gps_mapper.py](/code/gps_mapper.py)

The resulting plot should look similar to the one shown below, where the points have been parsed from the log file and plotted atop an open street map as red dots:

![GPS Coordinates Mapped](/images/gps_tracker_screenshot.png)

