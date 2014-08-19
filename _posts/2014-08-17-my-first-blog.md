---
layout: post
title: My first blog on Github!
tags: [testtag]
---

I have been interested in writing blogs on Github for a while. However after poked around in some articles on the Internet, I gave up since they had always asked to setup Jekyll environment locally first (I have so many client devices...) 

Until yesterday, after read one article [Build A Blog With Jekyll And GitHub Pages](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/), within one hour, I could set my blog site up in Github very easily. I really thank the author for sharing his work.

Next, I will explore the possibilities for using my blog repository with Eclipse (since I'm Eclipse guy) and how to add comments, subfolders in my Github blog site: 

With Eclipse, I can use EGit to manage my blog repository. I also installed a Markdown plugin from Eclipse markplace. But I haven't found a Jekyll plug for Eclipse yet. 

Then I found two lines in "_config.yml" file:  
`# Your disqus shortname, entering this will enable commenting on posts`  
`disqus:` 

After I registed in disqus.com and got a shortname, I put it in above line, save and push it into Github. I waited for seconds and refreshed this blog page, I could see the commenting box. It's a quick setting and wonderful!!!



