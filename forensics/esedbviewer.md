---
layout: forensics
title: EseDbViewer
---

# EseDbViewer #

## Info ##

Extensible Storage Engine (ESE) is one of the least known and yet most widely distributed database engines (on Windows). ESE is also known as JET Blue, is an Indexed Sequential Access Method (ISAM) data storage technology from Microsoft. 

ESE is notably a core of Microsoft Exchange Server and Active Directory. Its purpose is to allow applications to store and retrieve data via indexed and sequential access. Windows Mail and Desktop Search on Windows Vista also make use of ESE to store indexes and property information respectively. It is now also used within Windows Live Messenger. I only care about ESE from a forensics point of view, since some interesting data could be stored in an ESE database like a suspects document paths or their entire Windows Live Messenger contacts list. Rather than making one tool to work with the Windows Live ESE database and one for the Desktop Search etc, I thought it would make more sense to create a database data viewer with special features for some of the apps that use ESE e.g. Windows Live Messenger, Desktop Search and Windows Mail. 

When you open an ESE database you get to choose the "Mode" which currently consists of Generic, Desktop Search and Windows Live Messenger. If you choose the Windows Live Messenger mode option and (obviously) open a Contacts.edb file, then rather than giving you access to every field of every table, only the "SimpleContacts" table is shown, with only the key fields shown. Then when exporting data you only have the key data shown rather than every column etc. 

If you use the application to view the Desktop Search database (Windows.edb), then I recommend that you extract the entire "WindowsSearch" directory tree, since ESE uses extra files to store transactions and logs. 

The application uses a managed wrapper (http://www.codeplex.com/ManagedEsent) to access the ESE functionality as it’s pretty dirty to use, well from a nice, safe C# point of view! :-) 

Some example paths for the *.edb files are shown below: 

- Windows Live Messenger: C:\Users\woany\AppData\Local\Microsoft\Windows Live Contacts\{5dabbe1a-86f7-47af-92d9-8228549cb5d9}\DBStore 
- Desktop Search: C:\ProgramData\Microsoft\Search\Data\Applications\Windows 
 
## Errors ##

If you get a **JET_errFileAccessDenied **error then it may be related to not having administrative rights or UAC is inferring. 

## Screenshots ##

## Download ##

[v1.05](http://www.woanware.co.uk/downloads/EseDbViewer.v.1.0.5.zip)