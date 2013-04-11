---
layout: misc
category: misc
title: wpic
---

# {{ page.title }} #

## Info ##

wpic is a simple console web page capture tool based on the Chromium project that allows for the entire page to be captured as an image... 

    Usage: wpic.exe -u "http://www.woanware.co.uk" -o woanware.png` 

wpic can now process against URL's that can be altered by the app, so you could do something like the following which will perform a query against google, using the values from the input file, pausing for 1000 MS between each one, because we are nice:
  
    wpic.exe -u "https://www.google.com/search?q=#DATA#" -i "C:\Input.txt" -p 1000

## Screenshot ##

## Download ##
- [Binaries (v1.0.1)](/downloads/wpic.v.1.0.1.zip)