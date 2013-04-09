---
layout: default
title: USBDeviceForensics
---

# USBDeviceForensics #

## Info ##
USBDeviceForensics is an application to extract numerous bits of information regarding USB devices. It uses the information from a SANS blog posting to retrieve operating system specific information. It now has the ability to process multiple NTUSER.dat registry hives in one go. 

It should be noted that whilst the information in the blog posting is accurate, there is a caveat to be aware of. During my testing I have found that an unknown process can update the Date/Time values across all keys, in particular the USBSTOR keys. Therefore, you could see the same Last Written Date/Time value on each device key. If you see this occurring, then you obviously cannot rely on the values retrieved. All of the dates should be UTC. 

It is possible to set a time zone offset by using the Time Zone window e.g. Tools->Time Zone menu item. The Install date time zone appears to be the local time zone.
 
## Download ##

- [Binaries (v1.0.11)](/downloads/USBDeviceForensics.v.1.0.11.zip)