title: shimcacheparser
link: http://www.woanware.co.uk/?page_id=515
creator: woany
description: 
post_id: 515
post_date: 2012-10-23 19:04:42
post_date_gmt: 2012-10-23 19:04:42
comment_status: closed
post_name: shimcacheparser
status: publish
post_type: page

# shimcacheparser

This is a .Net port of the Mandiant ShimCacheParser ([https://github.com/mandiant/ShimCacheParser](https://github.com/mandiant/ShimCacheParser)). This project is written for .Net 4.5 and requires Visual Studio 2012. The obvious difference is that it is written in C#, and it does not support data extraction from the local machine, nor from Mandiants MIR XML format, since I don't need this functionality. There are a number of reasons for porting, primarily to understand the SHIM cache format better, and this would not be possible without the excellent work from Andrew Davis (Mandiant). The second was two other tools I used displayed strange artifacts after the main binary path information. The final reason was that I wanted automated sorting and user defined delimiters! [https://github.com/woanware/shimcacheparser](https://github.com/woanware/shimcacheparser) **Download** [v1.0.1](/downloads/shimcacheparser.v.1.0.1.zip)