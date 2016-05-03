---
layout: post
categories: [jQuery, PHP]
tags: [jQuery, PHP, Twitter API]
excerpt_separator: <!--more-->

title: Political Grid Project
---

{: .center}
![Political Grid Project](/images/pgp/pgp_banner.png)

**Political Grid Project** is an analysis tool that measures general consensus of politicians' public statements, in particular politicians' tweets. As the most popular micro-blogging service, Twitter has played a significant role in defining social trends and influencing people’s political stances. The popularity of a Twitter user, including politician, oftentimes is measured by the number of tweets, retweets, mentions, and/or followers. We believe that these parameters do not provide enough information about where the public stands on a political remark. To follow a politician does not necessarily imply that he or she supports that politician. Moreover, the number of retweets and mentions may not suggest high level of consensus. In order to overcome these limitations and to further analyze the complexity of Twitter, Political Grid Project provides a mechanism in which a user can vote on political tweets based on two parameters: agree/disagree and important/ not important. This tool allows the user to examine his or her political stance and accordance with politicians, parties, and other political bodies.
<!--more-->

System Architecture
-------------------

**Political Grid Project** is build upon multi-tiered client-server architecture, in which the client only displays data that has been queried to the server. Furthermore, the server also acts as a proxy that communicates to the Twitter servers since majority of Twitter API does not support cross domain AJAX call. Both server side and data access layer are written in PHP. The client side is fully AJAXified in order to enhance user experience. It also utilizes Twitter REST API to gather tweet information. The database functions are fully parameterized in order to prevent SQL injection.

{: .center}
![Political Grid Project's System Architecture](/images/pgp/pgp_system_context.png)

**Political Grid Project** was a part of my senior design (capstone) project at Georgia Institute of Technology. My teammates and I created this website to help [Tanyoung Kim](http://www.tanykim.com/) with her research. She wanted to analyze "how people engage in data generation, how they explore the data through visualization, and what insights they obtain through these holistic exploration". The project was developed on Spring 2012, and it is based on Agile development methodology.

***Disclaimer:*** I no longer contribute in version after beta release.

External Link
-------------

* [Political Grid Project Website](http://politicalgrid.gatech.edu/)
* [Project documentation](/resources/pgp/Political_Grid_Project_Documentation.pdf)
