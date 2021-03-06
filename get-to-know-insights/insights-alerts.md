---
title: SysKit Alerts
description: The SysKit Insights Alerts page gives you an overview of your alerts. 
author: Tomislav Sirovec
date: 19/02/2018
---

The SysKit Insights Alerts page gives you an overview of your alerts. There are three categories:

## Performance Counters

Performance Counters tab will automatically populate as soon as the application concludes the status's of the performance counters. That usually happens within 15 minutes of starting the application. 
The columns we provide here are: Farm, Server, Counter, Instance, Avg. Value, Time. A __red__ square in front of the server name indicates that the counter is in __Critical__ state. __Yellow__ square indicates a __warning__ status.  
Clicking on any Performance Alert will open a detailed view on the right hand side of the window. There you can find more information about the specific Performance Counter. Such as its description, the defined values for the thresholds, and the graph with the collected values. For more information on how to manage the alerts, [see this article](#internal/how-to/manage-alerts).


## Events

Events tab will be populated as soon as you define a __new Alert__. For more information on how to do this, [click here](#internal/how-to/manage-alerts). 

The columns we provide here are: Farm, Server, Name, Query, Time.
The square in the Server column is always grey and is indicative of Events Alert.
Clicking on a Events Alert will open the details on the right hand side, which will show you the results of the defined query. Clicking on the __View Details__ will preselect the query and take you to the Event Viewer screen.

## SharePoint Status

SharePoint Status tab will automatically be populated. By default SysKit Insights checks the SharePoint Timer Service status and the Central Administration (CA) site status. If the Timer Service job is stopped or the CA is unavailable, you will be notified every 30 minutes.  
The columns we provide here are: Farm, Server, Source, Value, Time.
See the [Manage Alerts](#internal/how-to/manage-alerts) article to see how you can check the status of another site.  

> __Please note!__ - To check (ping) a SharePoint site we are using the credentials of the service account you provided during the configuration of the SysKit Insights. Also, it is not possible to use forms authentication. 

## Sending the notification

In order to receive the email notification of your alerts you need to enable them. Go to Settings -> Email settings. Select the: "Send email notifications when alerts occur" and fill out all the required fields.  

---
>For more information on Insights features [see this article.](https://www.syskit.com/products/insights/features/intelligent-alerts/)