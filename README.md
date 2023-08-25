# RaspberiPiTouchScreenConfig
Config file for the Adafruit 5" and 7" 800x480 TFT HDMI Backpack

Create file on the Pi at /boot/config.txt

The important bit is:
```
hdmi_group=2
hdmi_mode=87
hdmi_cvt=800 480 60 6 0 0 0
hdmi_drive=1

max_usb_current=1
```

Set `hdmi_drive=2` for RPi 4

Also on Raspberry Pi — use the raspi-config tool to force audio to the 3.5mm jack (not HDMI or auto). Not all screens support audio over HDMI, and in this case it may actualy interfere with the display.


Ref:
https://learn.adafruit.com/adafruit-5-800x480-tft-hdmi-monitor-touchscreen-backpack/raspberry-pi-config
