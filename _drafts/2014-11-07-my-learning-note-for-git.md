---
layout: post
title:  How to Use Git
tags: 
- git
categories:
- development
---

There are a lot of similar blogs, articles on the Internet already. This blog is only my note, if you have a article with the same name, I'm sorry about it. 

Currently, my department plans to use Atlassian Stash (git repository server) to replace our SVN repository. 

Some colleagues in the team ask me to provide some training or introduction about Git since they know I has been used it.

In fact, I don't think I'm an expert at it, I have learned and continuously learn it on the Internet. But I do have some Git experience to share: 

1. first of all, understanding the basic concepts and related operations:
   local work copy
   index
   remote repository vs local repository
   
   Please read the following materials to understand them: 
   
   head  (is the last commit-pointer in the current working branch )[http://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell#_git_branching]
   How does Git know what branch you’re currently on? It keeps a special pointer called HEAD. Note that this is a lot different than the concept of HEAD in other VCSs you may be used to, such as Subversion or CVS. In Git, this is a pointer to the local branch you’re currently on
   
   local repository
   local branch
  
   remote branch (pointer to the branch in the remote repository)
   tracking branch (upstream, mapping between remote branch and local branch for push upstream and featch upstream)
   
   
   basic operations: 
   
   add, commit, reset, checkout, ignore
   clone
   merge,
   pull fetch + merge (if tracking branch is set up
   push
   rebase
   
   fast-forward vs (+) force update
   
   The + tells Git to update the reference even if it isn’t a fast-forward.
   
   Because a branch in Git is in actuality a simple file that contains the 40 character SHA-1 checksum of the commit it points to, branches are cheap to create and destroy. Creating a new branch is as quick and simple as writing 41 bytes to a file (40 characters and a newline).
  

   
    fast-forward and basic merge: http://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
    
    Generally it’s better to simply use the fetch and merge commands explicitly as the magic of git pull can often be confusing.
    
    rebase: http://git-scm.com/book/en/v2/Git-Branching-Rebasing
    In general the way to get the best of both worlds is to rebase local changes you’ve made but haven’t shared yet before you push them in order to clean up your story, but never rebase anything you’ve pushed somewhere.
  
  advanced concepts: 
    
  The Refspec 
  
  fetch = +refs/heads/*:refs/remotes/origin/*
	push = refs/heads/master:refs/heads/qa/master
      fetch: source (local branch in remote repository): target (remote branch)
      push:  source (local branch): target (local branch in remote repository)
      
  refs/heads; refs/remotes/origin/ see .git directory
  
  

   git work flow: https://www.atlassian.com/git/tutorials/comparing-workflows
   
   pull request

For understanding the basic concepts, there are a lot of resource on the Internet, the following is my favorits: 

http://git-scm.com/book/en/v2/Getting-Started-Git-Basics

http://stackoverflow.com/questions/3689838/difference-between-head-working-tree-index-in-git



2. secondly, create an account in [github]() or [bitbucket](), 

3. then, use a git client tool to create a git repository on github or bitbucket

'''
There are a lot of tools in the market. However I use EGit at the most of time since I said that I'm a fan of Eclipse. 
The only con for me to use EGit so far is that I have to add my each git repository into Eclipse as a Eclipse project.
'''

4. next, create a repository locally or remotely

5. finally, create a file, make a commit into repository (locally and remotely) and  practice and practices...

During above learning process, if find any issue or have question, Internet is the best trainer and teacher!

 