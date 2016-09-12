---
title: Patterns
keywords:
sidebar: framework_sidebar
permalink: patterns.html
toc: true
summary:
---

## [MICROSERVICES PATTERNS](http://microservices.io/patterns/index.html)
* [Database per service](http://microservices.io/patterns/data/database-per-service.html)
* [Event-driven architecture](http://microservices.io/patterns/data/event-driven-architecture.html)
* [Event sourcing](http://microservices.io/patterns/data/event-sourcing.html)
* [Microservice chassis](http://microservices.io/patterns/microservice-chassis.html)
* [Service instance per container](http://microservices.io/patterns/deployment/service-per-container.html)
* [Backend For Frontend (API Gateway)](https://www.thoughtworks.com/insights/blog/bff-soundcloud)
* [Server-side service discovery](http://microservices.io/patterns/server-side-discovery.html)
* [Self Registration](http://microservices.io/patterns/self-registration.html)


## STABILITY PATTERNS (INTEGRATION) PATTERNS
> Reliability in distributed systems is determined by the weakest component, so even a minor internal function could bring your entire system down. Learn how stability patterns anticipate the hot spots of distributed network behavior

* 'Use Timeouts' pattern
* 'Circuit Breaker' pattern
* 'Handshaking' pattern
* 'Bulkheads' pattern

Source: [Stability patterns applied in a RESTful architecture](http://www.javaworld.com/article/2824163/application-performance/stability-patterns-applied-in-a-restful-architecture.html)

## Strangler Pattern
> "The most important reason to consider a strangler application over a cut-over rewrite is reduced risk. A strangler can give value steadily and the frequent releases allow you to monitor its progress more carefully. Many people still don't consider a strangler since they think it will cost more - I'm not convinced about that. Since you can use shorter release cycles with a strangler you can avoid a lot of the unnecessary features that cut over rewrites often generate."
<br> -- Martin Fowler

Source: [Martin Fowler](http://www.martinfowler.com/bliki/StranglerApplication.html)

## Facade Pattern
> The facade pattern (or façade pattern) is a software design pattern commonly used with object-oriented programming. The name is by analogy to an architectural facade.

> A facade is an object that provides a simplified interface to a larger body of code, such as a class library. A facade can:

> * make a software library easier to use, understand and test, since the facade has convenient methods for common tasks;
* make the library more readable, for the same reason;
* reduce dependencies of outside code on the inner workings of a library, since most code uses the facade, thus allowing more flexibility in developing the system;
* wrap a poorly designed collection of APIs with a single well-designed API.

> The Facade design pattern is often used when a system is very complex or difficult to understand because the system has a large number of interdependent classes or its source code is unavailable. This pattern hides the complexities of the larger system and provides a simpler interface to the client. It typically involves a single wrapper class which contains a set of members required by client. These members access the system on behalf of the facade client and hide the implementation details.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Facade_pattern)

## Further Reading
* [Stability patterns applied in a RESTful architecture](http://www.javaworld.com/article/2824163/application-performance/stability-patterns-applied-in-a-restful-architecture.html)
* [Microservice architecture](http://microservices.io/index.html)
