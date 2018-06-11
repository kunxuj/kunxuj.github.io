---
layout: post
title: Writing my first Github blog without installation of Jekyll locally!
tags: [jekyll]
---

I have been interested in writing blogs on Github for a while. However after poked around in some articles on the Internet, I gave up since they had always asked to setup Jekyll environment locally first (I have so many client devices...) 

Until yesterday, after read one article [Build A Blog With Jekyll And GitHub Pages](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/), within one hour, I could set my blog site up in Github very easily. I really thank the author for sharing his work.

Next, I will explore the possibilities for using my blog repository with Eclipse (since I'm an Eclipse guy) and how to add comments, tags in my Github blog site: 

* Using Eclipse   
With Eclipse, I can use EGit to manage my blog repository, and I also installed a Markdown plugin from Eclipse markplace. But I haven't found a Jekyll plug in for Eclipse yet. 

* Using comments
There are two lines in "_config.yml" file:  
`# Your disqus shortname, entering this will enable commenting on posts`  
`disqus:`  
After I registed in disqus.com and got a shortname, I put it in above line, save and push it into Github. I waited for seconds and refreshed this blog page, I could see the commenting box. It's a quick setting and wonderful!!!

* Using Google Analytics  
There are two lines in "_config.yml" file: 
`# Enter your Google Analytics web tracking code (e.g. UA-2110908-2) to activate tracking`
`google_analytics: ` 
Same as using comments: register in Google Analytics site and get your tracking code, then add it after the colon. 

* Using tags
It seems that currently there is no built-in support for tagging in jekyll without using plug-ins. Here is [the ticket](https://github.com/jekyll/jekyll/issues/867). However, I found that [this article](http://www.minddust.com/post/tags-and-categories-on-github-pages/) provides a workaround. I follow the steps in it to configure this blog site, this is the reason why you can see a "test tag" tag at the end of this blog:-)

So far so good without installation of jekyll locally.


