
A simple WiFi based cat collar based of a Esp8266

The idea is that it will scan for wireless networks and if the cat is closer to networks 
that are not it's home network then it will beep, vibrate and flash a RGB LED. 

To save power. If the cat is at home the module will sleep for 5 minutes before scanning again. 

If other networks as visible during a scan then this is posted back to a local web server to 
triangulate that cats position or the direction the cat went.


Features:
-Esp8266
-USB LiPo charging
-USB Uart for programming/data
-WS2812 RGB led 
-Speaker (Buzzer)
-28x38mm board size
-3v3 i2c addon support, could add a MPU-9250 for gyroscope, accelerometer, compass
-Batery monitoring
-OTA software updating
