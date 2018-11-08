# Why Erlang?

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/erlang/why_erlang/illustrations/why_erang_001.png)

The choosing of any technology should be based on the issue that need to be solved. This article is covering reasons for choosing Erlang but not other languages in case of developing:

* payments system equipped or not by [blockchain](https://github.com/ArboreusSystems/arboreus_articles/tree/master/blockchain) tech
* fault tolerant data storage systems of different capacity for storing ([data storage, big-data storage, etc](https://github.com/ArboreusSystems/arboreus_articles/tree/master/data_storage))
* any log systems that is requiring to manage huge amount of events or handle a lot of types of events ([envent driven systems](https://github.com/ArboreusSystems/arboreus_articles/tree/master/event))
* etc

If necessary, the list of project types might be indefinitely prolonged, but every point of this list will be contained overall property - every project is over of abilities of one server, all of this project going to be DISTRIBUTED through the servers. And every servers will interact to others by sending messages.

The key-point - THE DISTRIBUTED. The ERLANG FROM BEGIN the language for developing DISTRIBUTED applications. The virtual machine of this language contain mechanism that is allowing servers interaction from begin. Developers don't need to reinvent the wheel, it's already invented and perfectly working. You might to choose any language that you want, but at time of writing this article only Erlang has in-box this kind of mechanism.

Briefly, the explanation of "Why Erlang?" might be something like this - **THE LANGUAGE FROM BEGIN FOR DISTRIBUTED APPLICATIONS**.

Beside all of it there are ability to use this mechanism for distributing C/C++ applications. You might to get it by your own in article [Erlang NIF](http://erlang.org/doc/tutorial/nif.html). You might to develop application modules on C/C++ and using Erlang like wrapper for distributing.

Based on experience of developing distributed applications - the  best way to use Erlang like primary language (the developing on Erlang is really faster then on any other) and if it not enough by any reason implement C/C++ modules. In case of necessity you might to write out the wrapper on C/C++ that will allow you to use Java application. But! It will look like trying to motivate turtle to improve the speed for the level of Formula 1.
