---
layout: post
title:  The Note for Learning Git
tags: 
- git
- tools
categories:
- development
---


Currently, my department plans to use [Atlassian Stash](https://www.atlassian.com/software/stash) (Git repository management server) to replace current SVN repository server. 

Some colleagues in the team ask me to provide some training or introduction about Git since they know I has been used it privately.

I don't think I'm an expert at it, I have just learned and continuously learn it on the Internet. 

However, I do have some Git experience to share. The following is my note for learning Git which I shared to my teammates: 

###1. First of all, understanding the following concepts and related operations:

   - Basic concepts:   

>  (local) Work directory  
>  Index  
>  HEAD   
>  remote repository vs local repository

>  Basic operations: add, commit, reset, clone, ignore

   The reference [here](http://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified) provides very easy understanding of most of above concepts and operations
   
   - Middle (level) concepts
   
>  branches: local (tracking) branch, remote (tracking) branch   
   `tracking branch (also be called as upstream branch, mapping between remote branch and local branch for push upstream and fetch upstream)`
   
>   Basic operations: checkout, branch, merge, rebase,  pull (= fetch + merge), push
   
   - Advanced concepts: 
   
>   Refspec,   
>   .git/config   
>   [Git work flows](https://www.atlassian.com/git/tutorials/comparing-workflows)

###2. Secondly, create an account in [github](https://github.com/https://bitbucket.org) or [bitbucket](https://bitbucket.org), and create a remote repository on them.  


###3. Then, use a Git client tool to manage a local Git repository (either clone from above remote repository or create from scratch in the local environment)  
    
There are a lot of tools in the market. However I use EGit since I always use Eclipse manage my projects (remember? As I have said that I'm a fan of Eclipse and I think EGit is really a great Git tool).   
    The only con for me to use EGit so far is that I have to add my each git repository into Eclipse as a Eclipse project, and I don't want some files to be a part of a Eclipse project.

###4. In addition, add or update files in local repository and try the basic operations: add, commit, push, fetch, pull, etc.  

###5. Practice and practice...

   During the practices, if find any issue or have question, Please remember that Internet is the best trainer and teacher! The followings resources are my favorites online resource for learning Git: 

- [Pro Git book](http://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

- [Git tagged questions in stackoverflow](http://stackoverflow.com/questions/tagged/git)

- [EGit User Guide](http://wiki.eclipse.org/EGit/User_Guide)
    


  

 

 