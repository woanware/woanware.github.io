---
layout: forensics
category: forensics
title: TargetAnalyser
---

# {{ page.title }} #

## Info ##
TargetAnalyser is basically a rip off of [Automater](http://www.tekdefense.com/automater/), which is a python script designed to perform URL/Domain, IP Address, and MD5 Hash OSINT tool aimed at making the analysis process easier for intrusion Analysts. 

The issue for me is that sometimes I want to look at the page that produced the output, so a UI provides an easy way to get all the info and yet still provide a quick method to open the page. I have also added a lot more OSINT.

## Features ##

- IP Void (IP)
- URL Void (URL)
- Robtex (A Records)
- Fortiguard (IP/URL)
- AlienVault (IP/URL)
- Malware Domain List (IP/URL)
- VxVault (Hash)
- MinotaurAnalysis (Hash)
- ThreatExpert (Hash)
- VirusTotal (Hash)
- BFK Passive DNS
- VirusTotal (DNS)
- HpHosts (IP/URL)
- Hurricane Electric (IP)

## Third party libraries ##

- [DNS](http://www.codeproject.com/Articles/23673/DNS-NET-Resolver-C): DNS lookups
- [ObjectListView](http://objectlistview.sourceforge.net/cs/index.html) : Data viewing via lists 
- [VirusTotal.NET](https://github.com/woanware/VirusTotal.NET): Fork from https://github.com/Genbox/VirusTotal.NET
- [Utility](http://www.woanware.co.uk): Misc functions (woanware)

## Requirements ##

Microsoft .NET Framework 4.5

## Download ##

- [Source Code](https://github.com/woanware/TargetAnalyser)
- [Binaries (v0.0.10 - Console)](/downloads/TargetAnalyser.v.0.0.10.Console.zip)
- [Binaries (v0.0.10 - GUI)](/downloads/TargetAnalyser.v.0.0.10.GUI.zip)
