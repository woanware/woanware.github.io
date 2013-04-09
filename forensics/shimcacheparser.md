---
layout: default
title: shimcacheparser
---

## shimcacheparser ##

This is a .Net port of the Mandiant ShimCacheParser ([https://github.com/mandiant/ShimCacheParser](https://github.com/mandiant/ShimCacheParser)). 

This project is written for .Net 4.5 and requires Visual Studio 2012. The obvious difference is that it is written in C#, and it does not support data extraction from the local machine, nor from Mandiants MIR XML format, since I don't need this functionality. 

There are a number of reasons for porting, primarily to understand the SHIM cache format better, and this would not be possible without the excellent work from Andrew Davis (Mandiant). 

The second was two other tools I used displayed strange artifacts after the main binary path information. The final reason was that I wanted automated sorting and user defined delimiters! 

## Download ##
- [Source Code](https://github.com/woanware/shimcacheparser)
- [Binaries (v1.0.1)](/downloads/shimcacheparser.v.1.0.1.zip)