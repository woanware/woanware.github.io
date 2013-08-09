---
layout: network
category: network
title: ftpcheck
---

# {{ page.title }} # 

## Info ##

Got bored logging into FTP services checking for anonymous authentication and whether I can have write privileges etc, so ftpcheck does it. 

There is a file within the applications directory that allows for various settings/defaults to be tweaked e.g. paths that are tested for, anonymous accounts used, users for enumeration. 

## Features ##

- Checks for anonymous authentication
- Checks for write privileges
- Attempts to retrieve the system details using the SYST command
- Retrieves the directory listing when connected
- Retrieves the current working directory using the PWD command
- Attempts some user enumeration using the "~" directory name format
- Attempts to retrieve the /etc/passwd file via path traversal
- Attempts to retrieve the .rhosts file
- Attempts to retrieve the boot.ini file via path traversal

## Example Output ##

    ftpcheck v1.0.0 

    [+] Quote help The following commands are recognized

    ABOR ACCT ALLO APPE CDUP CWD DELE FEAT HELP LIST MDTM
    MKD MODE NLST NOOP OPTS PASS PASV PORT PW QUIT REIN REST
    RETR RMD RNFR RNTO SITE SIZE SMNT STAT STOR STOU STRU 
    SYST TYPE USER XCUP XCWD XMKD XPWD XRMD HELP 
    command successful. (code=214) 

    [+] System Details (SYST): 
    [ ] Windows_NT 
    [+] Current Working Directory (PWD) 
    [ ] / 

    [+] Directory Listing 
    [ ] -rwxrwxrwx 1 owner group 22 May 9 15:51 New WinRAR ZIP archive.zip 

    [+] User Privileges 
    [ ] WRITE privileges 

    [+] User Enumeration 
    [ ] ~root does not exist 
    [ ] ~oracle does not exist 
    [ ] ~bin does not exist 

## Download ##

[Binaries (v1.0.7)](/downloads/ftpcheck.v.1.0.7.zip)