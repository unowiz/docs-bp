---
title: Number of Web Applications
description: Number of Web Applications best practices report by SPDocKit determines whether the number of web applications in the farm is in accordance with Microsoft recommendations.
author: Matija Hanzic
date: 23/6/2017
tags: Windows SharePoint Services 3.0,SharePoint Server 2007,SharePoint Foundation 2010,SharePoint Server 2010,SharePoint Foundation 2013,SharePoint Server 2013,SharePoint Server 2016
---
### Issue description
This check determines whether the number of web applications in the farm is in accordance with Microsoft recommendations.

### Explanation
SharePoint web applications are logical abstractions on top of IIS websites. One SharePoint web application can consist of multiple IIS sites and content databases (where site collections are stored). Additionally, a number of timer jobs are created for each SharePoint web application. This creates overhead and requires more hardware to run fluidly. Therefore, it is recommended that the number of SharePoint web applications is kept below 20 for each SharePoint farm.

Creating new web applications is recommended in the following scenarios:
* Web applications with different authentication methods (different IIS application pools)
* Dedicated web application for My Sites site collection

### Solution
Creating multiple SharePoint web applications is unavoidable, but because they create a lot of overhead it is recommended to keep the number to a minimum. When applicable create an additional host-named site collection instead of web applications.

### Additional information 
Additional information can be found in the following article:
* [Web application limits](https://technet.microsoft.com/en-us/library/cc262787%28v=office.16%29.aspx?f=255&MSPPError=-2147217396#WebApplication)