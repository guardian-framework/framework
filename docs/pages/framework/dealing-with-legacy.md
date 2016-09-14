---
title: DEALING WITH LEGACY
keywords: Legacy
sidebar: framework_sidebar
permalink: dealing-with-legacy.html
toc: true
summary: In computing, a legacy system is an old method, technology, computer system, or application program, “of, relating to, or being a previous or outdated computer system.” Often a pejorative term, referencing a system as “legacy” often implies that the system is out of date or in need of replacement.
---

<br>

> "Let's face it, all we are doing is writing tomorrow's legacy software today. By making it easy to be strangled in the future, you are enabling the graceful fading away of today's work."
<br> -- Martin Fowler

## Important Pages Relating To This One
* [Standardizations](standardizations.html)
* [Patterns](patterns.html)
* [Principles](principles.html)

## What Is a Legacy System?
In computing, a legacy system is an old method, technology, computer system, or application program, "of, relating to, or being a previous or outdated computer system." Often a pejorative term, referencing a system as "legacy" often implies that the system is out of date or in need of replacement.

While this term may indicate that some engineers may feel that a system is out of date, a legacy system may continue to be used for a variety of reasons. It may simply be that the system still provides for the users' needs. In addition, the decision to keep an old system may be influenced by economic reasons such as return on investment challenges or vendor lock-in, the inherent challenges of change management, or a variety of other reasons other than functionality. Backward compatibility (such as the ability of newer systems to handle legacy file formats and character encodings) is a goal that software developers often include in their work.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Legacy_system)

## Which Systems Are Legacy Systems?
![Cloud Native or Legacy](images/cloud-native-or-legacy.svg)

## The Law of Holes
> The first law of holes, or the law of holes, is an adage which states that "if you find yourself in a hole, stop digging". The meaning behind it is that if you find yourself in an untenable position, you should stop and change what you are doing, rather than carrying on and exacerbating the situation.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Law_of_holes)

## How To Handle Legacy Systems?
* Follow the "Law of holes" and stop digging!
* Legacy systems should only be maintained
  * Don't implement new functionality (improvements on current functionality is ok) in the legacy system
* Focus on stability and cost efficiency
  * Changes must not jeopardize the stability of the system
  * Changes must focus on stability and cost efficiency
  * All changes to infrastructure, tools and code must be justified based on maintenance alone
* The legacy systems should be "made irrelevant" not changed, with the use of
  * Strangler Pattern
  * Facade Pattern
  * (Possibly) API Gateway Pattern

## Putting The Strangler And Facade Pattern To Practical Use
* The Strangler Pattern must be controled by the new development
* New development must be greenfield ([Being Cloud Native](being-cloud-native.html)) i.e. it should not have any knowledge of the legacy systems except for the facade
* A Facade Pattern must be implemented by the legacy team to hide the legacy system

## Implementing A Facade Pattern With API Management
* This applies **ONLY** to legacy systems that can not expose APIs according to [Cloud Native](being-cloud-native.html)
* API Management hides the complexity of the legacy systems and make them look and feel [Cloud Native](being-cloud-native.html) while at the same time not forcing them to change their methods of integration
* The API Management system **MUST NOT** be used as part of ANY greenfield development

## Implementing Strangler Pattern With Only A Request Reuter
* In the best of all worlds the request coming in is a http request and in that case it's preferable to implement the strangulation via a Request Reuter
* A Request Reuter can be a Layer 7 load balancer or a reverse proxy

## Implementing Strangler Pattern With A Microservice, Behind An API Gateway Pattern, Behind A Request Reuter
* Sometimes it's not as easy as just reuting a request and than the recommend way is to implement a Microservice (greenfield) behind a API Gateway pattern
* The API Gateway pattern should in turn be behind a Request Reuter to help with future strangulations

## How to access data from the legacy system by the new service
* Try to avoid the need for accessing/providing data between the new and the old
  * When it's necessary, Invoke a remote API provided by the legacy systems facade

## Further Reading
* [DDD Surrounded by Legacy Software](http://domainlanguage.com/ddd/surrounded-by-legacy-software/)
* [Refactoring a Monolith into Microservices](https://www.nginx.com/blog/refactoring-a-monolith-into-microservices/)
* [Strangler Applications](http://paulhammant.com/2013/07/14/legacy-application-strangulation-case-studies/)
* [API Management](https://azure.microsoft.com/en-us/services/api-management/)
