---
layout: default
category: forensics
title: ForensicUserInfo
---

# ForensicUserInfo #

## Info ##

After the previous post regarding Windows user passwords, I have now after quite a lot of work created ForensicUserInfo, which is a GUI tool that allows you to import registry files (requires the SAM, SOFTWARE and SYSTEM hives) and then extracts the user information from the various files and then decrypts the LM/NT hashes from the SAM file.The application can export the information to either CSV or HTML. 

There is now a console version that generates text output. This would not have been possible without the posting at the [Push the Red Button](http://moyix.blogspot.com/2008/02/syskey-and-sam.html) blog regarding the SYSKEY and the SAM file. The process used to encrypt/obfuscate the password hashes is a joke, in that it is over the top, since once you have the files (SAM and SYSTEM) then you can get the hashes. 

ForensicUserInfo will extract the following information: 

- RID
- Login Name
- Name
- Description
- User Comment
- LM Hash
- NT Hash
- Last Login Date
- Password Reset Date
- Account Expiry Date
- Login Fail Date
- Login Count
- Failed Logins
- Profile Path
- Groups

## Download ##
- [v1.0.1](/downloads/forensicuserinfo.console.v.1.0.1.zip) Console
- [v1.0.4](http://www.woanware.co.uk/downloads/ForensicUserInfo.v.1.0.4.zip) GUI