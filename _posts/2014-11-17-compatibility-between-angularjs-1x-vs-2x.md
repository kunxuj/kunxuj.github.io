---
layout: post
title:  Compatibility Issues Between AngularJS 1.x and 2.x 
         - Rethink Angularjs as the Client MVC Framework
tags: 
- angularjs
- client mvc
categories:
- frontend
- architecuture
---

In our team, we have been used server side MVC such as Struts, JSF, Spring MVC, etc. for very long time.  They are very stable, very mature, but they tightly mixed server logic with presentation code. Sometimes it's not convenient to enhance or improve the front end code. So, I have planed to take advantage of loose coupling of the architecture of "restful API + client mvc" in my Team.    

Among many client mvc frameworks, AngularJs is my first choice due to many [merits](http://www.sitepoint.com/10-reasons-use-angularjs/)    

However, during ngEurope meeting last month, Augularjs team  provided some thoughts and plan for Augularjs future version 2.0, here is the some references about that meeting and Angular2.0: 
 
<http://www.michaelbromley.co.uk/blog/267/my-thoughts-on-ngeurope-2014-and-angularjs-2-0>    
<http://angularjs.blogspot.ca/2014/03/angular-20.html>

It's not new that the new version of AngularJS 2.0 will be different from old 1.x. However the upset news is that the new version may be a potential lack of backwards compatibility or easy migration path.  

This is really not good news for existing users and prospective users like me. 

In the following articles and their comments, some existing users expressed their upset.

<http://developer.telerik.com/featured/can-angularjs-maintain-dominance/>   
<http://www.theguardian.com/info/developer-blog/2014/nov/10/on-the-ambitious-but-bumpy-road-to-angularjs-20>


For users like me, It's a dilemma: 

    1. If I plan to use the current version (1.3) now, I can't explain if my team-mates ask me why to use this framework which will soon be deprecated and has no smooth path to be upgraded to the newer version.    
    2. If I plan to wait for the newer version (2.x), it will be available at least half a year later. 
   
Even though I still like AngularJS, I have to rethink to use it. Maybe it's time to review other frameworks: BackboneJs, EmberJs, KnockoutJs, etc.
   
   
