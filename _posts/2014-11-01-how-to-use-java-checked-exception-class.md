---
layout: post
title:  How to Use Java Checked Exception Classes
tags: 
- Exception
categories:
- java
- development
---

If we search "java checked Exception vs unchecked Exception" on the Internet, there are a lot of debates about which one is better and should be used. 

Though, I think the most of unchecked Exceptions should be found during testing and debugging processes (there are indeed some exception cases). I don't want to attend the above debates and compare both in this article. I just want to use this article to share my some experience about to how to use checked Exception classes in our code. 

In classes hierarchy in one application, if an exception occurs from the lower layer or the bottom of the hierarchy,  there are following steps to handle it:      

* Developers should make sure where to handle the Exception 

* If it can be handled by developers and end users not need to know, then handle it and log it in the middle of the hierarchy 

* If developers don't known how to handle or it�s better to let end users know the exception, try to handle it if possible, log and display exception message (which should be understandable to end users) on UI layer - the highest layer in the hierarchy (for end users). 

There are two ways to create Exception classes in the application: 

* Create as few exception classes as possible: using a general exception class with different exception messages for one category exceptions (different exception messages will differentiate the exceptions). 

* Create as detailed exception classes as possible, using different exception classes for different exceptions in one category

Note: If need to display exception messages to end users, exception messages may need to be converted to the ones that end users can easily understand, there are possibly two ways: 

* Using exception code for the exception message is easy to convert later on the UI (highest) layer since codes (unique) are easier to be compared than string messages (may difficult to be unique)

* If the exception classes are very specific, it�s easy to convert  messages based on the class name on the UI (higher) layer

In some situation, when we handle the unchecked Exceptions from the third party package or Web Service end point, we may run into some complexity, but above principles should be the same. 