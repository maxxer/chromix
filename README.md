Chromix
==========

This tool is a Zabbix Trigger Check tool.  
When Trigger is "PROBLEM", this tool generate Desktop Notification.

This tool uses Zabbix API.

You can register Multi Zabbix Servers to this tool.  
So, when you manage many zabbix server, you may be happy.

I tested the following environments:
Zabbix Server
 - ver.1.8.3
 - ver.1.9.8
 - ver.2.0.0RC2
 - ver.2.0.0

Chrome
 - 19.0.1084.41 beta-m
 - 22.0.1229.14 beta

How to Use
-----------

### 1. Prior Work

This app is using Zabbix API,  
So, you should give API access authority.

* Zabbix 1.8:
    * Belong to "API access" group the users that you want to access.
* Zabbix 2.0:
    * It is not necessary to the above work.
    * You just have to give access to the host to the user.

Please check the official document.  
[Zabbix Official Manual](http://www.zabbix.com/documentation/)

### 2. Installation

Please install the Chromix from the Chrome Web Store.  
[Chromix-Chrome Web Store](https://chrome.google.com/webstore/detail/odjpdjeegacmncmodjbeboldofhljjjf,"Chromix")

### 3. Registration of Zabbix info

* Click Chromix icon on your chrome tool bar.
* Click "Add Zabbix".
* Fill in data about Zabbix.
    * If your Zabbix top url is "http://hostname/zabbix", the url column is filled in the box to this format "hostname/zabbix". 
    * If your Zabbix use "https", please check "SSL?" box.

### 4. Check the trigger

After this configure, chromix start monitoring trigger which status is "problem" automatically .
(Number of list item is only 100.)

### 5. Background

Chromix count the number of problems that occurred up to the current time from the last check of chromix.  
So, When you check the popup once, the number is reset.

### 6. Settings

At the chromix option page, you can set Desktop Notification feature.  
If you want to use Desktop Notification function, Please Click "On".

At this page, you can also change Background check rate and Notification display time.  
Default setting is 20 seconds.

License
-------
Copyright 2012 Daisuke Ikeda (dai.ikd123@gmail.com)

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

