---
title:  "Response to A List of Things"
date:   2016-09-20 10:18:00
description: HTML Article Response
---

I've been hearing about how websites are still not optimized and it loads slowly. 
This article states that we're not doing a good job on page-load times. 
The problem seems to lie down to websites that are not so responsive mostly because the designers were lazy. 
Mostly because of single code base trying to solve problems for every platforms.

When requests to visit a website, Computer users basically get initial request pings back and forth from 
the user's local DNS, and then to the host server.
Therefore, there is a delay to visit a website because a browser and a web server has to exchange data. 
Mobile devices on the other hand usually has to go through a service tower first before contacting DNS sever.
Because of this, there are more delays for mobile dvices to visit a website even though LTE and 4G connections today
are blazing fast and it somewhat compensates the performance delays.

Browsers recieve chunks of HTML files from the server and parses them to display. However, parsing HTML with extra files
such as javascript and CSS would prolong the process even more. Blocking is a methods to help HTML files to load quicker.
Blocking is when CSS and Javascript requests are blocked when page is loading. This is usually achieved by blocking rendering for
CSS to help the UI to load consistently. Not sure how this could be achieved, and I'm guessing I have a lot to learn.

