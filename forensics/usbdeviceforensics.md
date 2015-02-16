---
layout: forensics
category: forensics
title: USBDeviceForensics
---

# {{ page.title }} #

## Info ##

usbdeviceforensics is a python script to extract numerous bits of information
regarding USB devices. It initially used the information from a SANS blog
(Rob Lee) post to retrieve operating system specific information. It now
has the ability to process multiple NTUSER.dat registry hives in one go.

The python script was originally a Windows only .Net application but I decided 
that it was pointless having a GUI for this applicaton.

It should be noted that whilst the information in the blog posting is
accurate, there is a caveat to be aware of. During my testing I have found that
an unknown process (probably an update) can update the Date/Time values across
all keys, in particular the USBSTOR keys. Therefore, you could see the same
Last Written Date/Time value on each device key. If you see this occurring,
then you obviously cannot rely on the values retrieved. All of the dates should
be UTC.

## Installation ##

This script needs the [python-registry](https://github.com/williballenthin/python-registry) module created by Will Ballenthin

- Install git python python-dev
- sudo pip install enum34
- git clone https://github.com/williballenthin/python-registry.git
- cd python-registry
- sudo ./setup.py install

The GUI .Net version (v1.0.14) is now deprecated.
 
## Download ##

- [Python with deps (v0.0.1)](https://github.com/woanware/usbdeviceforensics/releases/download/v0.0.1.deps/usbdeviceforensics.v0.0.1.with.deps.zip)
- [Python (v0.0.1)](https://github.com/woanware/usbdeviceforensics/releases/download/v0.0.1/usbdeviceforensics.v0.0.1.zip)
- [Source Code](https://github.com/woanware/usbdeviceforensics)
- [Binaries (v1.0.14)](/downloads/USBDeviceForensics.v1.0.14.zip)