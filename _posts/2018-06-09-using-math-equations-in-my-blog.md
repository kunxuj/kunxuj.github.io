---
layout: post
title:  Using Math Equations In My Blog
tags: 
- jekyll
categories:
- tools
- website
---

Preparing to write some blogs with a lot of complicated math equations, I found a good way to go: 

-  Using Jupyter Notebook to write a markdown article with math equations 

     Note: MathJax in Jekyll site supports "$$" escape characters, but not "$"  

-  Download the "ipynb" file as a markdown file
-  Copy the downloaded markdown file to "_posts" folder of this site.  
-  Add the the YAML front matter block as other posts 

The following is some examples of math equations: 

$$L^{CLIP}(\theta) = \hat{\mathbb{E}}_t [\min(r_t(\theta) \hat{A}_t, \text{clip}(r_t(\theta), 1 - \epsilon, 1+\epsilon) \hat{A}_t)]$$

$$\max_{\theta} \quad L_{old}(\theta)  \\
s.t. \quad \bar{D}_{KL}(\theta_{old}, \theta) \leq \delta$$

Originally, I planed to use Microsoft OneNote 2016. Its math equations handwriting recognition feature is very impressive. However, since it can not easily be converted into Latex format and have to use image for the equations, I gave up. 

To let my Jekyll site to support math equations, I did the following modification on my website: 

- Make sure to use Kramdown markdown engine (defualt engine for Jekyll)
- Add the following line in the "_layouts/default.html" to support MathJax: 

```
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
```

In addition, since I have to upgrade this 4 years old Jekyll site to the latest version (from version 2 to 3), I also did some changes to fix the incompatible issues (please see the change log in the Github repo). 

