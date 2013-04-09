---
layout: default
title: l2tViewer
---

# l2tViewer

**Info** 

Note: l2tViewer is still **BETA** software. Some parts are rough around the edges, some bits might not work etc. l2tViewer uses .Net 4.5 so it is time to upgrade your .Net install :-) All of my future releases will be recompiled with .Net 4.5 so you may as well upgrade now: 

- Bootstrap: http://go.microsoft.com/fwlink/?LinkId=225704 
- Standalone: http://go.microsoft.com/fwlink/?LinkId=225702 

l2tViewer is designed to improve timeline analysis for the output produced by the excellent [log2timeline](http://code.google.com/p/log2timeline/). 

Viewing, sorting CSV files via spreadsheet software does not work well due to the volumes of data involved in modern timeline analysis, which is where l2tViewer comes in. 

It is designed to be fast when importing with minimal overhead and dependencies. l2tViewer uses a MS SQL Server 2012 LocalDB instance to store the data. 

LocalDB needs to be installed (just use all of the default options) before running: 

- x86: http://download.microsoft.com/download/8/D/D/8DD7BDBA-CEF7-4D8E-8C16-D9F69527F909/ENU/x86/SqlLocaLDB.MSI 
- x64: http://download.microsoft.com/download/8/D/D/8DD7BDBA-CEF7-4D8E-8C16-D9F69527F909/ENU/x64/SqlLocalDB.MSI The application currently imports about 200,000 records  in 25 seconds on an $MFT file and 350,000 records in 55 seconds on a mixed Windows file. 

**Usage**

  * Click the File->New menu item or New tool bar button, select output folder, wait for the DB to be generated.
  * Next click the File->Import->Single menu item, choose the log2timeline file, the app will load a few lines to preview it
  * Enter the Mount Point Prefix, mine is generally something like "[root]\" or "/mnt/windows_mount/", this value will be replaced with a mounted image (as a local drive) e.g. "D:\" for file viewing and hashing, click OK and wait for the import to finish
  * Click the Tools->Set Drive menu to choose the already mounted forensic image, then the context menu items will be enabled, so you can then right click on a row and choose the View or Hash context menu items
  

**Screenshot** ![](/wp-content/uploads/Main2.png) 

**Download** [v0.0.3](/downloads/l2tViewer.v.0.0.3.zip)