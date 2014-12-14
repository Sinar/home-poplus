---
layout: post
title:  "Sinar Project's Popit implementation: Introduction"
author: Ng Swee Meng
date: 14-12-2014
categories: post
published: false
---

Sinar Project is a non profit group that use technology to make information accessible to the people. We have a number of project, one of these is MyMP project that is done with collaboration of UndiMsia!, a voter education group, to build a database of members of parliament of Malaysia. 

MyMP project goal is to educate the people on the members of parliament of the area they live in. We do it by asking opinion on current issue to Members of Parliament, and at the same time collect past work on these people. We have a few version of the people database created, unfortunately it is very API driven and UndiMsia! is not a technical group. In the end of the day we decide to make one with Plone, because volunteer from MyMP project from UndiMsia! that will interview the Members of Parliament and add into the site. A CMS will work better now than an API based app without UI. 

While the MyMP project is successful in their own way, being included in google election page for Malaysia during the last general election for example. The data is not complete and we still hope to have an API so that software developers will adopt our data to make something useful. So we are in search of a better solution

We stumble upon Poplus project which Dave Whiteland introduce to us. Dave found us when our developer Chee Leong have done a pull request for AduanKu our FixMyStreet instance(But that is story for another day). After evaluation we found it that it fit our requirement for 3 reason. 
1) It have an RESTful API for people to integrate in their project.
2) It UI that lay person can use for data entry. 
3) It is build on top of Open standard. It allows independent implementation, and a way to integrate with different application. 

With the flexibility and open source, we will stick with this for a long time. The next post will be about how we populate the data into our PopIt instance. 


