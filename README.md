# How to fix a Raspberry PI
All you need to fix your Raspberry PI. This guide is made for newbies and you don't need to be a software engineer or to own a PhD to fix your Raspberry PI!

## Troubleshooting guide

### Power ON your PI, what does happen?

* Nothing, the screen remains black but there is a green LED next to the power plug that is blinking 4 times and repeats. [Solution](#reset-config-file)

## Fix
### Reset config file
Explore the SD card using your computer and at the root of the SD card you should find a `config.txt` file. If it's empty it's because you unpluged the power supply before the Raspberry was properly shut down (stop doing that!). You can copy paste this in `config.txt`, save and put back the SD card in the Raspberry:
```
start_x=1
hdmi_drive=2
hdmi_group=1
hdmi_mode=16
```
