---
title: SharePoint Search Service Applications
description: SharePoint Search Service Applications best practices report by SPDocKit determines whether the total number of Search Service Applications is exceeding the supported limit.
author: Aleksandar Draskovic 
date: 23/6/2017
tags: Windows SharePoint Services 3.0,SharePoint Server 2007,SharePoint Foundation 2010,SharePoint Server 2010,SharePoint Foundation 2013,SharePoint Server 2013,SharePoint Server 2016
---
### Issue description
This check determines whether the total number of Search Service Applications is exceeding the supported limit.
### Explanation
Search Service Application provides the enterprise search functionality to one or more SharePoint farms. It provides mechanisms to index SharePoint and non-SharePoint content sources, query the indexed data and provide search results, where required. The search architecture contains search components and databases. How you structure the search architecture depends on where you intend to use the search: for the enterprise or for internet sites. 

When building the search architecture, you should take into account considerations such as high availability and fault tolerance, the volume of your content and the estimated amount of page views and queries per second.

Multiple SharePoint Search Service Applications can be deployed on the same farm, because you can assign search components and databases to separate servers. The recommended limit of 20 is less than the maximum limit for all service applications in a farm.
### Solution
You have to make sure that the number of Search Service Applications is within the supported boundaries. To check your service applications, go to the **Central Administration** > **Application Management** > **Manage service applications**.
### Additional information 
Additional information can be found in the following article:
* [Manage service applications in SharePoint 2013](https://technet.microsoft.com/en-us/library/ee704544.aspx)