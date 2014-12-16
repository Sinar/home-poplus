---
layout: post
title:  "How sinar import data to popit"
author: Ng Swee Meng
date: 18-12-2014
categories: post
published: false
---

To make popit useful the first step is to populate data on it. One thing that the MyMP site lack is complete data set for all Members of Parliament, another is it only have Members of Parliament but not the opposition leader of an area. We have approach to a local news portal MalaysiaKini, they have graciously provide use with a database dump of 2013 election candidate. The dataset is good enough to provide the relevant data on providing a basic profile of a election candidate of that election. 

To import the data from the database dump to PopIt we use the popit-python library [popit-python](https://github.com/mysociety/popit-python). Here is the comment from the developer that work on the data import:
* Populating `Person` and `Organization` field is easy with popit-python
* `Post` and `Membership` API are both very similiar which might prove confusing for some of the new users.  But I think a bit of documentation on the workflow will suffice.
* Record pagination is recently implemented. `Popit-python` at that time seems lacking examples but because the library is based on [Slumber](http://slumber.readthedocs.org/en/v0.6.0/), it inherited the functionality.
* No easy way to update Posts record on the web UI (But the API is good enough for third party UI development).
* The API will reject POST requests with empty value, example {"name":""}, found out later that it should be {"name":null}.


