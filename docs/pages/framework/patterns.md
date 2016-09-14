---
title: PATTERNS
keywords:
sidebar: framework_sidebar
permalink: patterns.html
toc: true
summary: In software engineering, a software design pattern is a general reusable solution to a commonly occurring problem within a given context in software design. It is not a finished design that can be transformed directly into source or machine code. It is a description or template for how to solve a problem that can be used in many different situations. Design patterns are formalized best practices that the programmer can use to solve common problems when designing an application or system.
---

## Microservices Patterns
* [Overview](http://microservices.io/patterns/index.html)
* [Database per service](http://microservices.io/patterns/data/database-per-service.html)
* [Event-driven architecture](http://microservices.io/patterns/data/event-driven-architecture.html)
* [Event sourcing](http://microservices.io/patterns/data/event-sourcing.html)
* [Microservice chassis](http://microservices.io/patterns/microservice-chassis.html)
* [Service instance per container](http://microservices.io/patterns/deployment/service-per-container.html)
* [Backend For Frontend (API Gateway)](https://www.thoughtworks.com/insights/blog/bff-soundcloud)
* [Server-side service discovery](http://microservices.io/patterns/server-side-discovery.html)
* [Self Registration](http://microservices.io/patterns/self-registration.html)


## Stability Patterns (Integration)
Reliability in distributed systems is determined by the weakest component, so even a minor internal function could bring your entire system down. Learn how stability patterns anticipate the hot spots of distributed network behavior

* 'Use Timeouts' pattern
* 'Circuit Breaker' pattern
* 'Handshaking' pattern
* 'Bulkheads' pattern

Source: [Stability patterns applied in a RESTful architecture](http://www.javaworld.com/article/2824163/application-performance/stability-patterns-applied-in-a-restful-architecture.html)

## Patterns for Enabling Change

### Strangler Pattern
"The most important reason to consider a strangler application over a cut-over rewrite is reduced risk. A strangler can give value steadily and the frequent releases allow you to monitor its progress more carefully. Many people still don't consider a strangler since they think it will cost more - I'm not convinced about that. Since you can use shorter release cycles with a strangler you can avoid a lot of the unnecessary features that cut over rewrites often generate."
<br> -- Martin Fowler

Source: [martinfowler.com](http://www.martinfowler.com/bliki/StranglerApplication.html)

### Facade Pattern
The facade pattern (or façade pattern) is a software design pattern commonly used with object-oriented programming. The name is by analogy to an architectural facade.

A facade is an object that provides a simplified interface to a larger body of code, such as a class library. A facade can:

* make a software library easier to use, understand and test, since the facade has convenient methods for common tasks;
* make the library more readable, for the same reason;
* reduce dependencies of outside code on the inner workings of a library, since most code uses the facade, thus allowing more flexibility in developing the system;
* wrap a poorly designed collection of APIs with a single well-designed API.

The Facade design pattern is often used when a system is very complex or difficult to understand because the system has a large number of interdependent classes or its source code is unavailable. This pattern hides the complexities of the larger system and provides a simpler interface to the client. It typically involves a single wrapper class which contains a set of members required by client. These members access the system on behalf of the facade client and hide the implementation details.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Facade_pattern)

### Feature Toggles
A feature toggle, (also feature switch, feature flag, feature flipper, conditional feature, etc.) is a technique in software development that attempts to provide an alternative to maintaining multiple source-code branches (known as feature branches).

Continuous release and continuous deployment provide developers with rapid feedback about their coding. This requires the integration of their code changes as early as possible. Feature branches introduce a bypass to this process. Feature toggles bring developers back to the track, but the execution paths of their features are still "dead" if a toggle is "off". But the effort is low to enable the new execution paths just by setting a toggle to "on".

The technique allows developers to release a version of a product that has unfinished features. These unfinished feature are hidden (toggled) so they do not appear in the user interface. This allows many small incremental versions of software to be delivered without the cost of constant branching and merging.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Feature_toggle)

### Canary Release
Canary release is a technique to reduce the risk of introducing a new software version in production by slowly rolling out the change to a small subset of users before rolling it out to the entire infrastructure and making it available to everybody.

Similar to a BlueGreenDeployment, you start by deploying the new version of your software to a subset of your infrastructure, to which no users are routed.

Source: [martinfowler.com](http://martinfowler.com/bliki/CanaryRelease.html)

### Blue-green Deployment

One of the challenges with automating deployment is the cut-over itself, taking software from the final stage of testing to live production. You usually need to do this quickly in order to minimize downtime. The blue-green deployment approach does this by ensuring you have two production environments, as identical as possible. At any time one of them, let's say blue for the example, is live. As you prepare a new release of your software you do your final stage of testing in the green environment. Once the software is working in the green environment, you switch the router so that all incoming requests go to the green environment - the blue one is now idle.

Source: [martinfowler.com](http://martinfowler.com/bliki/BlueGreenDeployment.html)
