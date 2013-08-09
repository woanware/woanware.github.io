---
layout: application
category: application
title: SqlServerDataExtractor
---

# {{ page.title }} #

## Info ## 

Sometimes we need to drop a binary onto a box and extract the data. This application allows you to specify the connection string and SQL statement. Once the SQL statement executed, the data is output to a file in the application directory, which is loaded into a browser control on the second tab. The reason for using HTML to display the data, is that the application should be flexible enough to handle alot of data... If you need help with SQL connection strings then check out: http://www.connectionstrings.com/ 

## Connection Strings ##

- Data Source=IP;Initial Catalog=DB;User Id=USER;Password=PASS;
- Data Source=IP\INSTANCE;Initial Catalog=DB;User Id=USER;Password=PASS;
- Data Source=IP;Initial Catalog=DB;Integrated Security=SSPI;
- Data Source=IP\INSTANCE;Initial Catalog=DB;Integrated Security=SSPI;
 
## SQL Statements ##

- select @@version
- select user_name()
- select db_name()
- select * from sysusers
- select * from sysobjects where type = 'U' order by name
- select id from sysobjects where name = 'TABLE_NAME'
- select name from syscolumns where id = ’123456789’

## Features ##

- Nice little progress bar
- Handles large volumes of data

## Download ##

[Binaries (v1.0.1)](/downloads/SqlServerDataExtractor.v.1.0.1.zip)