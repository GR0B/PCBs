## USB Protection ##
Robert Sturzbecher 2020

A simple USB protection module based around a Onsemi NCP361SNT1G to protect USB ports 
from over current and over voltage events. 



Why would you need this? Are USB port not already protected? 

Well if you are using a Raspberry Pi and you pull too much power it does cut the power but
before the first USB hub, which in turn takes out all USB devices. This includes the 
Ethernet as it is also a USB device. 
So the Pi will drop offline and fail to boot in these cases, and only sometimes a USB 
overcurrent message in syslog.


While the NCP361SNT1G does offer voltage and current protection, the "Alert FLAG Output"  
does not seem to flag OCP events (only OVLO/UVLO events).  


NCP361SNT1G datasheet [https://datasheet.lcsc.com/lcsc/1809111618_onsemi-NCP361SNT1G_C233714.pdf]