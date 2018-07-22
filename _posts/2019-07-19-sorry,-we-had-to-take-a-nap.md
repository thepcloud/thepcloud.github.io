---
layout: post
title:  "Sorry, We had to take a nap."
date:   2018-07-19 23:58:36 -0500
categories: jekyll update
permalink: /blog/sorry-we-had-to-take-a-nap
---
Last week Jitsi crashed because the [Videobridge](http://github.com/jitsi/jitsi-videobridge) couldn't keep up with the streaming from multiple rooms and multiple participants in addition to the other components required to run [Jitsi](http://jitsi.org) suite.

 There had been a tutorial posted by one of the [Jitsi Developers](https://community.jitsi.org/c/dev) on [YouTube](https://www.youtube.com/watch?v=LyGV4uW8km8&t=99s) the week before on how to properly configure  Videobridge to load balance when using the platform as [VCaaS](https://cloud.videxio.com/blog/5-things-to-consider-when-investing-in-videoconferencing-as-a-service-vcaas).  
 
 Luckily, after a little tweaking and adding another Videobridge droplet now [Jicofo](http://github.com/jitsi/jicofo) balances the servers evenly to keep them from crashing. I really think 4 Videobridges and 2 servers hosting [Prosody](http://prosody.im), [Jicofo](http://github.com/jitsi/jicofo), and [Jitsi-Meet](http://github.com/jitsi/jitsi-meet) components to evenly distribute their traffic as well would be the best bet. If one of those components fail it really does not matter how many Videobridges  have been deployed because they are essential components to the suite as well.

 So there are some things to consider and with all that being said the site is back up and able to host private parties.

 Please send an [email](mailto:adminATperv.cloud) or hit me up on [Twitter](http://twitter.com/pervcloud) with feedback both good and bad so I can make sure everything is working correctly.

 If there is anyone that might be interested in helping with setup of the WebRTC and other services which are slated to be launched within the next few weeks then please look me up on [Github](http://github.com/thepcloud), [Twitter](http://twitter.com/pervcloud), or [email](mailto:adminATperv.cloud).
