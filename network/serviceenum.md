---
layout: network
category: network
title: ServiceEnum
---

# {{ page.title }} #

## Info ##

ServiceEnum is a .Net console application to perform Windows service enumeration. It is built using the lowest version of .Net e.g. v1.1 for x86 and v2 for x64. It extracts various service details including: 

- Service Name
- Display Name
- Status
- User
- Startup
- Path
- Verifies if binary exists
- Extracts parameters
- Determines if a quoted path is used
- File binary permissions via Win32 Advapi32 GetFileSecurity
- Security Descriptor via Win32 Advapi32 GetSecurityInfo

## Download ##

- [Source Code](https://github.com/woanware/ServiceEnum)
- [Binaries (v1.0.1)](/downloads/ServiceEnum.v.1.0.1.zip)