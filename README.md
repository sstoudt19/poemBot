# poemBot

> printer + pi + python + poems. 

A raspberry pi connected to a thermal printer offers physical prints from a daily poetry website, http://poetry.lib.uidaho.edu/

Here is a little video: https://twitter.com/VandalPoem/status/704377485593432065 

Based on Adafruit IoT Printer, https://learn.adafruit.com/pi-thermal-printer/overview

Requires printer library from Adafruit Python-Thermal-Printer, https://github.com/adafruit/Python-Thermal-Printer


# Set Up

After setting up and testing the python main loop and poem printing, set it to load on boot by editing rc.local:

```sudo nano /etc/rc.local```

Add the terminal command to start the python script before the line "exit 0":

```
cd /home/pi/Python-Thermal-Printer
python vpodMain.py &
```




