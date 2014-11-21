---
layout: post
title:  Why A POC Prototype Is An Artifact for "software Architecture"
tags: 
- poc
categories:
- software architecture
---

POC means [Prove Of Concept]()
Artifact means ....
[software architecture]() means: 
If someone searches "software architecture" on the Google, most of results will show the following similar definition about "software architecture": 

   - it is a highest level of abstraction of a software system 
   - it is the description and documentation of the structure of a software system
 
The purpose of "software architecture" is to make the stakeholders (end users, project managers, designers and developers, system administrators, etc.) of a software system to understand the software system (in the following sections, if not be specially mentioned, "system" and "software system", "architecture" and "software architecture" will be used interchangeably) easily. 

Currently, in software industry, not like building industry, there isn't a single view of a system which can make different categories of stakeholders to understand the system easily. Therefore, ["4+1 architectural view model"](http://en.wikipedia.org/wiki/4%2B1_architectural_view_model) has been used for trying explaining the system from different stakeholders perspective. Since UML is the main language to describe this kind of model, software developers, designers or architects mostly use UML to model a software architecture with different diagrams.

No matter which tools or models are used to describe a software architecture. The final architectural deliverable artifacts for software architecture work always are: diagrams,tables, documents. Please see references [a] [1] and [b] [2] 

Those artifacts had been very good for our software architecture work, but are they good enough? 

After more projects become agile, we heard more and often the similar critics about "software architecture work":   

1. Architecture work takes too long time
2. There is a big gap between original software architecture and implemented one hidden in the delivered code. 

There are a lot of reasons behind them. one of the big reason, in my opinion, is that there are big gaps between user requirement and defined architecture, between defined architecture and real architecture hidden in the delivered code.
And those gaps can only be reduced or removed in the late implementation phase. 

Why those gaps can not be found early stage? Because the defined or planned architecture in the early phase can' be verified, tested during the early stage of analysis and design phase. It's easy to imagine how difficult to judge the correctness of the diagrams and documentations since it's difficult to put constraints on them.


However, A [proof of concept (POC)](http://en.wikipedia.org/wiki/Proof_of_concept), can,  if not completely fix above issues, at least, it can reduce above issues dramatically.  

Why? Because the POC does not only provide feasibility proof, it also provides the following benefits during architecture work:

1. It will be more easy to verify, validate and test on POC than diagrams and documentation
2. It will runs on specific environment, it's easy to add constraints on it
3. It will push architect to understand the requirement more carefully and more deeply so that it will reduce the gap between requirement and defined architecture
4. It will push architect to understand the bottleneck, major critical issues in the implementation more carefully and deeply so that I will reduce the gap between defined architecture and implemented code 

5. It will speed up architectural understanding by developers 

6. it will speed up development process if the POC can be used as development template for developers

It's not possible to implement a full-fledged POC like a final product during the early age of architectural analysis and design. POC should focus on critical parts of requirement and possible bottleneck or blockers of implementation. 
Depends on complexity and scope of delivered system, the POC itself may be simple or complex, However the goal of POC is that to make a demo system as close to the final production system as possible within short period of time.




references    
[1]: https://www.google.ca/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=software+architecture+artifacts   
[2]: http://pubs.opengroup.org/architecture/togaf9-doc/arch/chap35.html




Most often the stakeholders, especially end users can't make the decision about their requirment based on the above models and documentation, or very often they can't figure out what exact they asked for. After developer implemented the system, users will have more and accurate feedback based on implemented system. Since at this time, the deadline is approaching, developers have to change the code directly without update the related document. 

Above 4+1 model or other models or documentation can't resolve aforementioned issue. So what can we do?



  


