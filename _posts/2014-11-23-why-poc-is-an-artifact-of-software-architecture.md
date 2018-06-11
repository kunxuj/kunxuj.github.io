---
layout: post
title:  Why A POC Is An Artifact of "Software Architecture"
tags: 
- poc
categories:
- architecture
---

POC is the abbreviation of [proof of concept](http://en.wikipedia.org/wiki/Proof_of_concept).   
[Artifact](http://en.wikipedia.org/wiki/Artifact_(software_development)) is a deliverable.   

[Software Architecture](http://en.wikipedia.org/wiki/Software_architecture) has no strict definition. 
If someone searches "software architecture" on the Google, most of results will show the following similar definition about "software architecture":    

   - It is a highest level of abstraction of a software system 
   - It is the description and documentation of the structure of a software system
    
The purpose of "software architecture" is to make the stakeholders (end users, project managers, designers and developers, system administrators, etc.) of a software system to understand the software system easily and provides the direction for lower level design and implementation. In the following paragraphs, if not be specially mentioned, "system" and "software system", "architecture" and "software architecture" will be used interchangeably.    

So far, in software industry, not like building industry, there has not been a single view of a system which can make stakeholders with different backgrounds to understand the system easily. Therefore, ["4+1 architectural view model"](http://en.wikipedia.org/wiki/4%2B1_architectural_view_model) or other models have been used for trying to explain the system from different stakeholders' perspective. Since UML is the main language to describe this kind of models, software developers, designers or architects mostly use UML to model a software architecture with different diagrams.   

No matter which tools or models are used to describe a software architecture. The final architectural deliverable - artifacts for software architecture work always are: diagrams, tables, PPT or other documents. Please see references [1] [1] and [2] [2]     

Those artifacts had been very good for our software architecture work during last two decades, but are they good enough?    

Nowadays, after more projects become agile, we heard more and often the similar complaints about software architecture work:    

1. Architecture document can't reflect user requirement correctly   
2. The designed software architecture and the one hidden in the delivered code are different.   
3. Can't validate and test architecture work very well like we did for implemented code.  


I can't defend for our architects since very often, those complaints were true. Maybe there are a lot of reasons behind them. For example: users don't know what they want; the requirement changes too often and too quick, and the project schedule is so tight so that the designed architecture can't catch up with changed requirement and code; and the architectural diagrams, documents are difficult to be validated and tested via review process before implementation; etc.    

I agree that they are legitimate reasons, but can we, architects, do a better job to reduce these issues and improve the situation?   

The answer is "yes", and definitely, we can. A intuitive and not too difficult way is that besides the diagram, PPT, and other documents which we provided, we also provide a POC since

 A POC:       

1. is a more effective communication tool among stakeholders (especially, end users) and architects so that it can reduce requirement change in the late development phases

2. can force architects to understand the requirement more carefully and more deeply so that it will reduce the gap between requirement and defined architecture

3. can force architects to understand the bottleneck, major critical issues in the implementation more easily and early so that it will reduce the gap between defined architecture and implemented code 

4. is easy to be added constraints on it since it will runs in the specific environment and context, therefore it can be more easy to be verified, validated and tested than diagrams and other documents

5. can speed up developers to understand architecture with the combination of reviewing document and code

6. can speed up implementation process if the POC is used as the implementation template   


It's not possible to implement a full-fledged POC like a final product during the early stage of architectural analysis and design. POC should focus on business and technical critical parts of the system. Depends on complexity and scope of a delivered system and time for architectural work, the POC itself may be simple or complex, However the goal of POC is that to make a prototype system as close to the final production system as possible within a certain resource and time constraints during the architectural work.   

There is no silver bullet in the world, A POC is not an exception. However, If we deliver a POC as an artifact in our software architecture work, even we can't completely resolve architectural issues, at least, we can reduce them dramatically.   

   
[1]: https://www.google.ca/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=software+architecture+artifacts   
[2]: http://pubs.opengroup.org/architecture/togaf9-doc/arch/chap35.html

  