---
layout: post
title:  The Note for Learning Git
tags: 
- git
- tools
categories:
- development
---


Currently, my department plans to use Atlassian Stash (Git repository server) to replace our SVN repository. 

Some colleagues in the team ask me to provide some training or introduction about Git since they know I has been used it.

In fact, I don't think I'm an expert at it, I have just learned and continuously learn it on the Internet. 

However, I do have some Git experience to share, the following is my note for learning Git which I shared to my teammates: 

1. First of all, understanding the basic concepts and related operations:

   Basic: 
   
   local work directory
   index
   HEAD
   remote repository vs local repository
   
    Operations: add, commit, reset, clone, ignore
   
   
   branches: local (tracking) branch, remote (tracking) branch
  
    tracking branch (upstream branch, mapping between remote branch and local branch for push upstream and featch upstream)
   
    Operations: checkout, branch, merge, rebase,  pull (= fetch + merge), push
   
   Advanced: 
   
   Refspec, .git/config
   
   Git work flows: https://www.atlassian.com/git/tutorials/comparing-workflows
   

To understand above Git concepts, I had read a lot of Git articles/blogs on the Internet, the followings are my favorites: 

http://git-scm.com/book/en/v2/Getting-Started-Git-Basics

http://stackoverflow.com/questions/3689838/difference-between-head-working-tree-index-in-git
   

2. Secondly, create an account in [github](https://github.com/https://bitbucket.org) or [bitbucket](https://bitbucket.org), and create a remote repository on them.

3. Then, use a Git client tool to Manage a local Git repository (either clone from above remote repository or create from scratch on local environment. 

    There are a lot of tools in the market. However I use EGit during the most of time since I said that I'm a fan of Eclipse and I think EGit is really a great Git tool. 
    The only con for me to use EGit so far is that I have to add my each git repository into Eclipse as a Eclipse project.
'''

4. In addition, create or update files in local repository and try the basic operations: add, commit, push, fetch, pull, etc.  

5. Practice and practices...

    During the practices, if find any issue or have question, Please remember that Internet is the best trainer and teacher!


  

 

 