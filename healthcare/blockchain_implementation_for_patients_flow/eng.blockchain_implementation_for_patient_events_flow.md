# Blockchain implementation for patient events flow

This article based on materials published before in this repository:

* ["Event driven"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/event/event_driven/eng.event_driven.md)
* ["Event Driven for Healthcare"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/healthcare/event_driven_for_healthcare/eng.event_driven_for_healthcare.md)
* ["Blockchain"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/blockchain/eng.blockchain.md)

It's very important to read it for understanding things described below. This article is only adaptation of principles for the purpose of healthcare. The list of articles above is describing fundament for this example and it's 99% of technology description.

The first of all you need to understand why you are going to use blockchain solution. Is there way to avoid blockchain? Why avoid? Because any blockchain solution is always complex solution that will require you more at time of maintaining. What the matter of the problem that you going to solve by using blockchain?

In case of healthcare we always have the Events Flow where the patient is the main cause of events: receipts, doctors conclusion, examination results and etc. This events located on timeline and this position on timeline highly critical value and it's shell be not changed in future. And the body of event shouldn't be changed too.

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/bc_example_event_flow/illustrations/blockchain_007.png)

The solution for avoiding fraud described in precise in article ["Blockchain example. Events flow implementation."](https://github.com/ArboreusSystems/arboreus_articles/blob/master/blockchain/bc_example_event_flow/eng.bce_events_flow.md). This solution might be released on SQL-based or noSQL-based DB Engines. The author of this article been using it on Erlang/C because this kind of technology stack allow to handle any amount of data, from small to big-data because of scalability of Erlang VM.

If need to improve security additionally to blockchain, there are might be separated storing of logical and verification indexes.

Follow author updates on [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/)

Follow AR|BO|RE|US updates on [**Twitter**](https://twitter.com/ArboreusSystems) and [**Linkedin**](www.linkedin.com/company/arboreus-systems/)