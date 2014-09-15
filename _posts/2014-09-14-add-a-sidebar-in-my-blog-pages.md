---
layout: post
title: Add a sidebar in my blog pages
tags: [jekyll]
categories:
- website
---

Before I write more blogs, I think it's better to add a sidebar to my blog pages for better categorization of my blogs, like a lot of other blog sites do on the web. Since I'm not familiar to Jekyll and want to save time to write more blogs, so I plan to use existing code. After searching on the Internet for a while, finally I found [this site](http://blankego.github.io/index.html) is exactly what I want: it has categories, tags, years for categorizing. 

After have studied this site's code and tried for multiple times, I finally added my own sidebar. The following are the summaries for adding it:

##1. Local Jekyll environment
   
Since there are a lot of possible tweaks and tries, I think it's a good idea to set up my local (Mac OS X Mavericks) Jekyll environment first to save multiple Git commit and push (In my [first blog](http://kunxuj.github.io/my-first-blog/), I said I didn't want to set up a local Jekyll environment since I have different working PCs). 

I had ran into some problems when setup local Jekyll environment according to [Jekyll web site](http://jekyllrb.com/)

* There was an error when ran "gem install jekyll": The solution is to run "gem update --system" to update RubyGems   
* There was an error when ran "jekyll serve": The solution is to run "gem install github-pages"

##2. Pass parameters via URL to a Jekyll/Liquid template

When I used the sidebar, I wanted to click one category/tag to see a page only containing blogs for that particular category/tag. To do so, I had planed to pass a parameter via the clicked URL to the targeted Jekyll/Liquid template. However, after I had researched for a while, I had to give it up since the static Jekyll template can't support to accept a dynamic passed parameter. 

##3. Change the way to add a tag in the blog. 
In my [first blog](http://kunxuj.github.io/my-first-blog/), I mentioned that I had used some workround to add a tag for a post, which was too cumbersome. Now I use the method from  [this site](http://blankego.github.io/index.html), then adding a tag or category is very easy: just add a tag or catgory in the post prefix part, for example for this post: 

```
---   
layout: post   
title: Add a sidebar in my blog pages   
tags: [jekyll]   
categories:  
- website  
--- 
```  

##To do:
Although I'm very happy that my blog pages have a side bar, there are still some more works to be done to have a better user experience. When I have time, I will  

* Show the tags/categories in every post which contains them
* Try to use Javascript to control that only one category/tag/year will be shown when click a category/tag/year in a side bar (at the same time hide others).
* Try to add a number representing the total posts of a year in Archive section of sidebar.
* Try to update Style sheets to improve layout of the Blog pages. 

Please stay tuned. 



