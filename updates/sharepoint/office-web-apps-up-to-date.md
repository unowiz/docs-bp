---
title: Office Web Apps Up to Date
description: Office Web Apps Up to Date best practices report by SPDocKit determines whether all Office Web Apps servers are up to date.
author: Aleksandar Draskovic
date: 19/6/2017
tags: Windows SharePoint Services 3.0,SharePoint Server 2007,SharePoint Foundation 2010,SharePoint Server 2010,SharePoint Foundation 2013,SharePoint Server 2013,SharePoint Server 2016
---
### Issue description
This check determines whether all Office Web Apps servers are up to date.
### Explanation
Microsoft releases Office Web Apps updates to ensure that the bugs found in the product are fixed. In addition, new functionality may be introduced with updates. Therefore, it is important to patch Office Web Apps on regular occasions.

Although they are two separate products, make sure that SharePoint and Office Web Apps servers are running on the similar patch level to ensure maximal compatibility.
### Solution
To verify which build your Office Web Apps servers are running on, start the Windows PowerShell and run the following cmdlet:
```
(Invoke-WebRequest http://office web apps url/m/met/participant.svc/jsonAnonymous/BroadcastPing).Headers["X-OfficeVersion"]
```
You can also check the version number in the Version column in **Control Panel** > **Programs** > **Programs and Features**. To see the list of version numbers click here: [SharePoint 2013 Build Numbers](http://www.toddklindt.com/blog/Lists/Posts/Post.aspx?ID=346).
### Additional information 
Additional information can be found in the following articles:
* [Office Web Apps Server](https://technet.microsoft.com/en-us/library/jj219456.aspx)
* [Apply software updates to Office Web Apps Server](https://technet.microsoft.com/en-us/library/jj966220.aspx)
* [SharePoint 2013 Build Numbers](http://www.toddklindt.com/blog/Lists/Posts/Post.aspx?ID=346#OWA)