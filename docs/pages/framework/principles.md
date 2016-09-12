---
title: Principles
keywords:
sidebar: framework_sidebar
permalink: principles.html
toc: true
summary:
---

## Smart endpoints and dumb pipes
> When building communication structures between different processes, we've seen many products and approaches that stress putting significant smarts into the communication mechanism itself. A good example of this is the Enterprise Service Bus (ESB), where ESB products often include sophisticated facilities for message routing, choreography, transformation, and applying business rules.
> <br><br>
> The microservice community favours an alternative approach: smart endpoints and dumb pipes. Applications built from microservices aim to be as decoupled and as cohesive as possible - they own their own domain logic and act more as filters in the classical Unix sense - receiving a request, applying logic as appropriate and producing a response. These are choreographed using simple RESTish protocols rather than complex protocols such as WS-Choreography or BPEL or orchestration by a central tool.
> <br><br>
> The two protocols used most commonly are HTTP request-response with resource API's and lightweight messaging.

Source: [Martin Fowler](http://martinfowler.com/articles/microservices.html)

## Design for failure
> A consequence of using services as components, is that applications need to be designed so that they can tolerate the failure of services. Any service call could fail due to unavailability of the supplier, the client has to respond to this as gracefully as possible. This is a disadvantage compared to a monolithic design as it introduces additional complexity to handle it. The consequence is that microservice teams constantly reflect on how service failures affect the user experience. Netflix's Simian Army induces failures of services and even datacenters during the working day to test both the application's resilience and monitoring.

Source: [Martin Fowler](http://martinfowler.com/articles/microservices.html)
