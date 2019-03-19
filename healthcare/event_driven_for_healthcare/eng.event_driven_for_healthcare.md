# Event driven for healthcare

Based on article - "[Event Driven](https://github.com/ArboreusSystems/arboreus_articles/blob/master/event/event_driven/eng.event_driven.md)", it's better to read it before.

Any healthcare facility producing, storing, analyzing huge amount of information. Beside all of it, gathering information from huge list of sources (another facilities, medical devices, etc). Almost every piece of information have to be analyzed statically and dynamically in context of time prospective or complex (cross-reference) research by composing facts by events. Every kind of information has to be stored for the long time period. Any kind of information strictly depend on "When?" it happened.

The informational environment that is around any healthcare facility is extremely complex within dynamically changing relations between parts or actors. Any medical devices provider (producer) always trying to insist on theirs own data exchange format, because of business.

Any attempt to improve the application or data format will get huge problem of inheritance from previous activities stored in different manners and formats. New application usage might be blocked by this problem, therefore usage of modern technologies might be impossible.

It wasn't the whole list of problems attached to the healthcare informational environment. The list of most difficult problems is looking like:

- huge amount of kinds or models of information
- huge amount of sources of information
- requirement to store it for a long time period
- necessity to analyze it
- a lot of data from previous
- strict dependency on the time of situation that is described by event and the time when information came to the system
- strict requirement of logging activities of users or patients
- different medical facility using different application within different formats of data

Why the well developed event driven system might be solution for healthcare facilities:

- from begin this kind of system time-related system, any kind of events might be ordered by timeline within ability to analyze it
- from begin this kind of system allow to create a data model of events dynamically, some kind of "on-fly", it will solve the problems: different devices from different producers, different sources within different formats
- based on previous point you always able to adjust data model by creating inherited new one without affecting gathered information, if any sources change the format or data model there are ability to react on it instantly
- huge inheritance problems might be soled although by ability to make a data model dynamically, there are only necessity to write small driver out based on data model

For example: the EMR records might be included to the event driven system like one of the list of types of events and it will solve the problem of huge inheritance.

From the point of view of this article, well developed event driven system has to have:

- dynamically data model creating engine
- triggering system 
- reliable storage within ability to be scaled by demand
- search or analyze engine added to the storage
- secured transport layer for delivering or getting events from different sources or storage
- secured client side solution 

All of points of this article based on previous articles published by me over here. You might to read it.

Follow author updates on [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/)

Follow AR|BO|RE|US updates on [**Twitter**](https://twitter.com/ArboreusSystems) and [**Linkedin**](www.linkedin.com/company/arboreus-systems/)