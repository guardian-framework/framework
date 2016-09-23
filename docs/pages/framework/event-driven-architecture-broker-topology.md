---
title: EVENT-DRIVEN ARCHITECTURE BROKER TOPOLOGY
keywords: Event-driven Architecture Broker Topology
sidebar: framework_sidebar
permalink: event-driven-architecture-broker-topology.html
toc: true
summary:
---

## Defining Event-driven Architecture
<iframe width="560" height="315" src="https://www.youtube.com/embed/XohG9yQe3Ps" frameborder="0" allowfullscreen></iframe>

## Defining Broker Topology
![Broker Topology](https://www.safaribooksonline.com/library/view/software-architecture-patterns/9781491971437/assets/sapr_0203.png)

As you can see from the diagram, there is no central event-mediator component controlling and orchestrating the initial event; rather, each event-processor component is responsible for processing an event and publishing a new event indicating the action it just performed.

Source: [Software Architecture Patterns](http://www.oreilly.com/programming/free/files/software-architecture-patterns.pdf)

## Justification Of The Choices Made
The broker topology differs from the mediator topology in that
there is no central event mediator; rather, the message flow is distributed across the event processor components in a chain-like fashion through a lightweight message broker (e.g., ActiveMQ, HornetQ, etc.). This topology is useful when you have a relatively
simple event processing flow and you do not want (or need) central event orchestration.

Source: [Software Architecture Patterns](http://www.oreilly.com/programming/free/files/software-architecture-patterns.pdf)

## The Other Alternatives That Were Not Chosen
* Mediator topology

## Further Reading
* [Software Architecture Patterns](http://www.oreilly.com/programming/free/files/software-architecture-patterns.pdf)
* [Event-Driven Data Management for Microservices](https://www.nginx.com/blog/event-driven-data-management-microservices/)
