---
layout: network
category: network
title: NetworkScanViewer
---

# {{ page.title }} #

##Info##

NetworkScanViewer is a GUI application designed to help view the results of nessus (v4/v5) and nmap (v5/v6) scan results. It combines the functionality of both NessusViewer and NmapViewer. 

The application loads the scan data from nessus and nmap XML, does some data cleansing, then displays the results on the results list. The list data can be sorted by clicking on the column headers, so it is easy to order and locate particular information. 

There is also the ability to filter on specific information like host, port, service etc so it is easy to drill down to specific information. The export functionality exports using the data shown in the results list, so if you change the sort order or filter the results, then it is reflected in the export. 

It is also possible to permanently exclude scripts that just generate noise by right clicking on the item and selecting "Ignore Plugin" from the context menu. Excluded scripts can be re-added at any time by using the Options window.   

## Note ##

Nmap files must have an *.xml file extension to be imported and nessus files must have a *.nessus file extension

##Features ##

- Data cleansing
- Export to CSV and XML
- Sortable data columns
- Data Filtering
- Script excluding 
- Data paging to support large volumes of data
- ESENT database to support large volumes of data
  
##Screenshots##

##Supported Nessus Version##

To check whether the correct version of nessus export files is being used, open up the file in a text editor and look for the following in the file header, if it does not contain it then it is the wrong version:

    <?xml version="1.0" ?>
    <NessusClientData_v2>

##Download##

[Binaries (v1.2.3)](https://github.com/woanware/NetworkScanViewer/releases/download/v1.2.3/NetworkScanViewer.v1.2.3.zip)