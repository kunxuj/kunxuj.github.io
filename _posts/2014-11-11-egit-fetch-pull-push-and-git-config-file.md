---
layout: post
title:  Understanding of EGit "Push,Fetch, Pull" Operations
tags: 
- git
- egit
categories:
- tools
---

When I started to use EGit, I always got confused by the similar terms for the following operations in the EGit menu: 

**Push, Fetch, Pull**   

After I read [EGit user guide](http://wiki.eclipse.org/EGit/User_Guide) carefully, searched Internet and tried by myself, I have the following understanding: 

###Push: 

* Pushing to upstream:    
EGit Menu Path:  Team -> Push to upstream   
Configuration, there are two kinds of configuration:   

  * Configure 1:  Team > Remote > Configure push to upstream....    
      Which will add/update the following line in "remote.name" section in the .git/config file:  
      push = refs/heads/master:refs/heads/master
      
   
  * Configure 2: [Upstream configuration](http://wiki.eclipse.org/EGit/User_Guide#Upstream_configuration)    
       Which will add/update the section "branch.name" in the .git/config file

>  The configure 1 has higher priority than 2. If both are removed from .git/config file, the "Push to upstream" will be disabled in the menu.   

>   When configure 1 takes effect, it may push changes from several local branches. 
   When configure 2 takes effect, EGit only push changes from the current branch. 


- Direct Push:   
EGit Menu Path:  Team > Remote > Push...   
Configuration, there are two configurations:   
         
  * Using existing "push specification" :  Git Repository view->Reposity ->Remotes->remote-name(default "origin") ->Push URL -> (click context menu->Configuration push... )
  * Making the custom configuration
         
> In .git/config file, above configuration will be located in the section of "remote.name"
         
> Direct push may always push changes from different local branches based on configured push specification.

> After adding files in an empty local repository which was cloned from remote repository, the EGit will ask to make push configuration when try to push. 

* Pushing to a remote Branch:    
EGit Menu Path:  Team -> Push Branch...   
Configuration, there are two kinds of situation:   

  * situation 1:  If the branch already has configuration in .git/config file, the EGit will use existing configuration.    
  * situation 2:  If the branch has no configuration in .git/config file, the EGit will make and save configuration in the config file after push.    
      

###Fetch

* Fetch from upstream:     
EGit Menu Path: Team > Fetch from upstream  
Configuration:  Team > Remote > Configure Fetch from upstream....

* Direct Fetch:   
EGit Menu Path: Team > Remote > Fetch from...   
Configuration, there are two configurations:   
         
   * using existing "fetch specification" :  Git Repository view->Remotes->remote-name(default "origin") ->Fetch URL -> (click context menu->Configure Fetch....)
   * make the custom configuration


###Pull
* Pulling New Changes from Upstream Branch:  
EGit Menu Path: Team > Pull   
Configuration:  based on tracking branch configuration




##Additional Comments

The result of EGit Push, Fetch, Pull operations heavily relies on how Git global and repositories configurations. For how detailed Git configuration parameters affect the results, please refer to the following Git references:  
 
http://git-scm.com/docs/git-config   
http://git-scm.com/docs/git-push    
http://git-scm.com/docs/git-fetch   
http://git-scm.com/docs/git-pull   
 

In addtion, understanding of the following concepts also help understand above three operations: 

* [Branching](http://wiki.eclipse.org/EGit/User_Guide#Branching)

  -  General remarks about branches   
  -  [Upstream configuration](http://wiki.eclipse.org/EGit/User_Guide#Upstream_Configuration)
  -  [Branch Creation Dialog](http://wiki.eclipse.org/EGit/User_Guide#Branch_Creation_Dialog)


* [Git References](http://wiki.eclipse.org/EGit/User_Guide#Git_References)

* [Refspecs](http://wiki.eclipse.org/EGit/User_Guide#Refspecs)   
     
     A "refspec" is used by fetch and push operations to describe the mapping between remote Ref and local Ref, it further divided into the following two categories: 

   - [Fetch Refspecs](http://wiki.eclipse.org/EGit/User_Guide#Fetch_Ref_Specifications)    
   - [Push Refspecs](http://wiki.eclipse.org/EGit/User_Guide#Push_Ref_Specifications)







 