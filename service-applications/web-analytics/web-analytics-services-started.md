---
title: Web Analytics Services Started
author: Aleksandar Draskovic
description: Web Analytics Services Started best practices report by SPDocKit determines whether the Web Analytics Service Application is created and started in the farm.
date: 21/06/17
tags: Windows SharePoint Services 3.0,SharePoint Server 2007,SharePoint Foundation 2010,SharePoint Server 2010,SharePoint Foundation 2013,SharePoint Server 2013,SharePoint Server 2016
---
### Issue description

This check determines whether the Web Analytics Service Application is created and started in the farm.

### Explanation

Web Analytics Service Application instances should be configured and running. A properly configured Web Analytics Service Application allows you to collect, report, and analyze the usage and effectiveness of your SharePoint sites. By using these features, you can understand what users are doing and what information they want from a site.

Please note that the Analytics components moved from the standalone web application to the Search Service Application in SharePoint 2013.

### Solution

Verify that the Web Analytics Service Application is running in the farm. To verify that the service application is started and configured properly, go to __Central Administration__ > __Application Management__ > __Manage service applications__.

### Additional information

Additional information can be found in the following article:
* <a href="https://technet.microsoft.com/en-us/library/gg266382(v=office.14).aspx">Configure Web Analytics service application (SharePoint Server 2010)</a>