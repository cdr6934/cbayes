---
title: 'Tips to SQL Script Writing Success'
author: Chris Ried
date: '2017-06-05'
slug: tips-to-sql-script-writing-success
categories:
  - SQL
tags:
  - sql
  - tips
---

The longer I've worked  in software development, the more I have to stress the importance of developing a methodology of naming, version control, and organizing all the various scripts that have been written. 

Following are a couple tips of advice I've collected over the last five years. I've found them to be  crucial to implement and habitualize best practices that are similar to these. It will save you time and also will make you more efficient. 

* When creating a directory, turn it into a GIT repository. 

* When naming your SQL scripts, use a declarative at the beginning of the file name (i.e. **SELECT**_xxx_MMDDYYYY.sql)

* Always create a text block at the beginning stating purpose, name and date when the script was written

* Never hard code dates in your scripts; this will bite you eventually. 

* Simple is better. There is always the urge to make things more complicated than needed. 
