---
title: Language Packs Up to Date
description: Language Packs Up to Date best practices report by SPDocKit determines whether all deployed language packs are properly updated to reflect the SharePoint Service Pack version.
author: Aleksandar Draskovic
date: 19/6/2017
tags: Windows SharePoint Services 3.0,SharePoint Server 2007,SharePoint Foundation 2010,SharePoint Server 2010,SharePoint Foundation 2013,SharePoint Server 2013,SharePoint Server 2016
---
### Issue description
This check determines whether all deployed language packs are properly updated to reflect the SharePoint Service Pack version.
### Explanation
SharePoint Server uses language packs to provide multilingual functionality. Language packs contain various dynamic link libraries (.dll files), which contain resources translated to specific languages. Whenever SharePoint functionality is updated with service packs, language packs also get updated to reflect the changes in the functionality and provide localized resources.

When you install a service pack to your SharePoint farm, you will also need to install service packs for all language packs you have deployed to your SharePoint farm in order to provide the localization for all services and features updated with the service pack. Please note that this is not required for the deployment of the cumulative updates, as the cumulative update packs contain localized resources for all available languages.
### Solution
Please check the patch level of all components and language packs in the SharePoint environment. To verify the upgrade status of the SharePoint farm and servers in the farm, open the **Central Administration**, and in the **Upgrade and Migration** section, click **Check product and patch installation status** (SharePoint 2010 and 2013) and verify the build numbers. All components listed should run the same build number. In the case that some components are running the lower build number, please install the appropriate updates.
### Additional information 
Additional information can be found in the following articles:
* <a href="https://technet.microsoft.com/en-us/library/ff806325(v=office.14).aspx">SharePoint Foundation 2010 and SharePoint Server 2010: Install a software update (SharePoint Foundation 2010)</a>
* [SharePoint Foundation 2013 and SharePoint Server 2013: Install a software update (SharePoint 2013)](https://technet.microsoft.com/en-us/library/ff806338.aspx) 