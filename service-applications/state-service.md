---
title: State Service
author: Aleksandar Draskovic
description: State Service best practices report by SPDocKit determines whether the State Service Application is created or started in the farm.
date: 21/6/17
tags: Windows SharePoint Services 3.0,SharePoint Server 2007,SharePoint Foundation 2010,SharePoint Server 2010,SharePoint Foundation 2013,SharePoint Server 2013,SharePoint Server 2016
---
### Issue description

This check determines whether the State Service Application is created or started in the farm.

### Explanation

The State Service Application is used by various SharePoint components to store temporary data across HTTP requests. The following SharePoint components use State Service Application:

* InfoPath Forms Services
* SharePoint Server Chart Web Part
* Microsoft Visio
* Search Administration Crawl And Query Health Reports

### Solution

Verify that the State Service Application is running in the farm. To verify that the service application is started and configured properly, go to __Central Administration__ > __Application Management__ > __Manage service applications__.

### Additional information

Additional information can be found in the following article:

* <a href="https://technet.microsoft.com/en-us/library/ee704548(v=office.14).aspx">Manage the State Service (SharePoint Server 2010)</a>