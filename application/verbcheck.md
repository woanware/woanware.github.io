---
layout: default
category: application
title: verbcheck
---

# {{ page.title }} #

## Info ##

Performs simple HTTP requests to validate the web servers supported HTTP verbs... 

## Features ##

- Configurable port
- HTTPS support
- Logs to file
- Configurable HTTP verb support via Checks.xml (located in app dir)
- Authentication support e.g. Basic, NTLM etc

## Notes ##

If a check has Body content then a "Content-Length" header is automatically defined and therefore a "Content-Length" header node does not have to added the "Checks.xml" file 

## Download##

[Binaries (v1.1.1)](/downloads/verbcheck.v.1.1.1.zip)