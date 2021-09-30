# EMURR
EMURR, or **Exhibit Marker Uniform Resource Router** is a mobile closed loop platform for deploying digital media content to devices using WiFi in geographical areas that have lacking infrastructure and reception. The working prototype uses the following components:
- TP-Link Archer C1200 Router (12v/1amp)
- Raspberry Pi Zero W (5v/1.5amp)
- 12V/11000mAh DC Output Battery w/2.1mm x 5.5mm output
- MicroUSB Cable

###Installation Instructions
The Raspbery Pi Zero W is running [Raspberry Pi OS Lite](https://downloads.raspberrypi.org/raspios_lite_armhf/images/raspios_lite_armhf-2021-05-28/2021-05-07-raspios-buster-armhf-lite.zip) Kernel Version: 5.10. Once you have the the disc image mounted to an SD card you will need to run the following steps:
1. Create a text file inside boot and named it wpa_supplicant.text. Inside this file, write the following:
```
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
country=US
 
network={
ssid="Your network SSID"
psk="Your WPA/WPA2 security key"
key_mgmt=WPA-PSK
}
```


## CAD Models
Models for EMURR display CHDR branding and enable the router to be hung on a pull along cart or from a backpack. The critical dimension of the router mount is stored in the DXF file. 3MF files are better quality but the STLs are included for previewing purposes. 

### Print Settings
All of these files should be printed PETG to allow for some flexibility. 
- .4 Initial Layer Height
- .15 Layer Height
- 240/90deg extruder/bed temps
- 15% infill (gyroid or rectilinear) and no need for support structures
