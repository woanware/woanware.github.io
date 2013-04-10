---
layout: default
category: application
title: nnikto
---

# {{ page.title }} #

## Info ##

A console app to perform forced browsing checks against a web server. It is heavily based apon nikto (cirt) and wikto (SensePost). It contains semi-intelligent techniques to prevent false positives... 

## Features ##

- Tolerance algorithm level modification (-a)
- Multithreaded, so its quicker than nikto
- SSL support (-s)
- Configurable Port (wow) (-p)
- Semi-intelligent techniques to determine false positives
- The responses from items located can be saved for checking later, so you don’t manually have to go to the site and check :-) (-l)
- Add cgi directories (-c), use a pipe (|) to separate each like "-d bob|chicken|fred"
- Doesn't hog the CPU like wikto
- Supports Basic Auth, NTLM and Negotiate
- Supports cookies

## Download ##

[Binaries (v1.2.3)](/downloads/nnikto.v.1.2.3.zip)