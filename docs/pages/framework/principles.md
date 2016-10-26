---
title: PRINCIPLES
keywords:
sidebar: framework_sidebar
permalink: principles.html
toc: true
summary:
---

## Smart endpoints and dumb pipes
When building communication structures between different processes, we've seen many products and approaches that stress putting significant smarts into the communication mechanism itself. A good example of this is the Enterprise Service Bus (ESB), where ESB products often include sophisticated facilities for message routing, choreography, transformation, and applying business rules.

The microservice community favours an alternative approach: smart endpoints and dumb pipes. Applications built from microservices aim to be as decoupled and as cohesive as possible - they own their own domain logic and act more as filters in the classical Unix sense - receiving a request, applying logic as appropriate and producing a response. These are choreographed using simple RESTish protocols rather than complex protocols such as WS-Choreography or BPEL or orchestration by a central tool.

The two protocols used most commonly are HTTP request-response with resource API's and lightweight messaging.

Source: [Martin Fowler](http://martinfowler.com/articles/microservices.html)

## Design for failure
A consequence of using services as components, is that applications need to be designed so that they can tolerate the failure of services. Any service call could fail due to unavailability of the supplier, the client has to respond to this as gracefully as possible. This is a disadvantage compared to a monolithic design as it introduces additional complexity to handle it. The consequence is that microservice teams constantly reflect on how service failures affect the user experience. Netflix's Simian Army induces failures of services and even datacenters during the working day to test both the application's resilience and monitoring.

Source: [Martin Fowler](http://martinfowler.com/articles/microservices.html)

## Privacy by Design
In short, privacy by design means that each new service or business process that makes use of personal data must take the protection of such data into consideration. An organisation needs to be able to show that they have adequate security in place and that compliance is monitored. In practice this means that an IT department must take privacy into account during the whole life cycle of the system or process development.

Source: [eudataprotectionregulation.com](http://www.eudataprotectionregulation.com/data-protection-design-by-default)

## Privacy by Default
Privacy by Default simply means that the strictest privacy settings automatically apply once a customer acquires a new product or service. In other words, no manual change to the privacy settings should be required on the part of the user. There is also a temporal element to this principle, as personal information must by default only be kept for the amount of time necessary to provide the product or service.

Source: [eudataprotectionregulation.com](http://www.eudataprotectionregulation.com/data-protection-design-by-default)

## There's no future in on-premises IT -- it's time to move to the cloud
You won't be the first to make such an adjustment. Thomas Edison, who invented the earliest system for electricity distribution in 1880, initially used direct current (DC). He didn't want to adopt alternating current (AC), though it could use higher voltages with transformers to step it down for distribution to homes and businesses. Competitors like Westinghouse were all about AC, but Edison doubled down and waged a propaganda war against the technology, trying to ban AC -- even electrocuting animals publicly to demonstrate the danger of AC. Ultimately, as we know, he failed, and AC current became our norm.

Once you see technology going in a direction that's unstoppable, don't get in the way or try to stem the tide. Instead, get on board. The cloud train is here.

Source: [infoworld.com](http://www.infoworld.com/article/2610801/iaas/there-s-no-future-in-on-premises-it----it-s-time-to-move-to-the-cloud.html)

## You Build It, You Run It
“Giving developers operational responsibilities has greatly enhanced the quality of the services, both from a customer and a technology point of view. The traditional model is that you take your software to the wall that separates development and operations, and throw it over and then forget about it. Not at Amazon. You build it, you run it. This brings developers into contact with the day-to-day operation of their software. It also brings them into day-to-day contact with the customer. This customer feedback loop is essential for improving the quality of the service.”

-- Werner Vogels

Source: [safaribooksonline.com](https://www.safaribooksonline.com/library/view/programming-amazon-ec2/9781449303617/ch01s03.html)

## Automation is Key to Efficiency
* People should never do what a machine can do well enough at equal cost (today or in the near future)

## Always-On, Always-Available
* Twenty four hours a day, seven days a week; constantly (24/7 Service)
* 99.9% availability
  * No exception to that rule (i.e. no planned maintenance windows)!

## Never Build a Single Point of Truth
Here’s a concrete example, based on real client experiences.

Architects for an airline created a services-based architecture with a canonical Customer service, encapsulating everything known about customers.

This is a natural instinct of software design, the DRY (Don’t Repeat Yourself) principle, Single Source of Truth, and other good (but abstract) ideas.

Then, a volcano erupted in Iceland, disrupting air travel drastically. Customers of the airline flooded the support center with calls, asking if the disaster would affect their flight. And people holding tickets in unaffected parts of the world couldn’t board their planes (because, of course, ticket lookups involved Customer).

While the architecture made logical sense, it fell over during extraordinary circumstances.

While it might seem wasteful or perhaps even lead to duplication (gasp!), having multiple customer services (one to handle customer issues, one to handle boarding) would have served the business better.

Only by thinking about the operational aspects of architecture can you build more robust systems, which is one of the goals of microservice architectures.

Source: [nealford.com](http://nealford.com/memeagora/2015/03/30/architecture_is_abstract_until_operationalized.html)

## Architecture is Abstract Until Operationalized
Software architects have the responsibility to elucidate decisions about how systems fit together, often by creating diagrams, with varying degrees of pomp.

Diagrams have a vague air of certainty around them, a wafting aroma of mathematics. Thus, architects often fall into the trap of envisioning software architecture as an equation they must solve.

Much of the commercial tooling sold to software architects reinforces the mathematical illusion of certainty with boxes, lines, and arrows–graphs don’t lie!

While useful, these diagrams offer a two dimensional view, a snapshot of an ideal world, but we live in a four dimensional world.

To flesh out that 2D diagram, you must put specifics to it. The ORM label on the 2D diagram becomes Hibernate v4.2.17, evolving into a three dimensional view of the world.

When you have a plan on how to put that into production and upgrade it to the inevitable Hibernate v4.3.0.1 in six months, you’ve graduated to a four dimensional world.

Too many architects fail to realize that a static picture of architetcure has a short shelf life. The software universe exists in a state of constant flux, it is dynamic rather than static.

Architecture isn’t an equation but rather a snapshot of an ongoing process.

Source: [nealford.com](http://nealford.com/memeagora/2015/03/30/architecture_is_abstract_until_operationalized.html)

## Separation of Concerns
In computer science, separation of concerns (SoC) is a design principle for separating a computer program into distinct sections, such that each section addresses a separate concern.

A concern is a set of information that affects the code of a computer program. A concern can be as general as the details of the hardware the code is being optimized for, or as specific as the name of a class to instantiate. A program that embodies SoC well is called a modular program.

Modularity, and hence separation of concerns, is achieved by encapsulating information inside a section of code that has a well-defined interface. Encapsulation is a means of information hiding.

Source: [wikipedia.org](https://en.wikipedia.org/wiki/Separation_of_concerns)

## Principle of Least Knowledge
The Law of Demeter (LoD) or principle of least knowledge is a design guideline for developing software, particularly object-oriented programs. In its general form, the LoD is a specific case of loose coupling. The guideline was proposed at Northeastern University towards the end of 1987, and can be succinctly summarized in each of the following ways:
* Each unit should have only limited knowledge about other units: only units "closely" related to the current unit.
* Each unit should only talk to its friends; don't talk to strangers.
* Only talk to your immediate friends.

Source: [wikipedia.org](https://en.wikipedia.org/wiki/Law_of_Demeter)

## Keep It Simple, Stupid (KISS)
KISS is an acronym for "Keep it simple, Stupid" as a design principle noted by the U.S. Navy in 1960. The KISS principle states that most systems work best if they are kept simple rather than made complicated; therefore simplicity should be a key goal indesign and unnecessary complexity should be avoided. The phrase has been associated with aircraft engineer Kelly Johnson (1910–1990). The term "KISS principle" was in popular use by 1970.[4] Variations on the phrase include "Keep it Simple, Silly", "keep it short and simple", "keep it simple and straightforward" and "keep it small and simple".

Source: [wikipedia.org](https://en.wikipedia.org/wiki/KISS_principle)

## You Aren't Gonna Need It (YAGNI)
"You aren't gonna need it" (acronym: YAGNI) is a principle of extreme programming (XP) that states a programmer should not add functionality until deemed necessary. XP co-founder Ron Jeffries has written: "Always implement things when you actually need them, never when you just foresee that you need them."[5] Other forms of the phrase include "You aren't going to need it" and "You ain't gonna need it".

YAGNI is a principle behind the XP practice of "do the simplest thing that could possibly work" (DTSTTCPW). It is meant to be used in combination with several other practices, such as continuous refactoring, continuous automated unit testing, and continuous integration. Used without continuous refactoring, it could lead to disorganized code and massive rework. YAGNI's dependency on supporting practices is part of the original definition of XP.

Source: [wikipedia.org](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)

## Opportunistic Refactoring
"From the very beginning of when I started to talk and write about refactoring people have asked me how it should be incorporated into the wider software development process. Should there be refactoring phases in the software development lifecycle, what proportion of an iteration should be devoted to refactoring tasks, how should we figure out who should be assigned to refactoring duties? Although there are places for some scheduled refactoring efforts, I prefer to encourage refactoring as an opportunistic activity, done whenever and wherever code needs to cleaned up - by whoever."

-- Martin Fowler

Source: [martinfowler.com](http://martinfowler.com/bliki/OpportunisticRefactoring.html)

## Bring the Pain Forward

## Last Responsible Moment

## "Yesterday's Best Practice Becomes Tomorrow's Antipattern"

## Coding Architects

## Documentation and models should be generated not written and drawn

## Open Source First

## Do Continuous Deployment

## Deployment Does Not Equal Release

## Don’t Build, What Can Be Used or Bought

## First Principle

## Autonomy, Mastery & Purpose
To motivate employees who work beyond basic tasks, give them these three factors to increase performance and satisfaction:
<br><b>Autonomy</b> — Our desire to be self directed. It increases engagement over compliance.
<br><b>Mastery</b> — The urge to get better skills.
<br><b>Purpose</b> — The desire to do something that has meaning and is important. Businesses that only focus on profits without valuing purpose will end up with poor customer service and unhappy employees.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Drive:_The_Surprising_Truth_About_What_Motivates_Us)

## Hire Only Polyglot Programmers
It’s common for people to be sceptical of software developers with varied coding experience. We’re used to seeing, “5 years C# experience” on the CV in front of us, so when we see a CV that says: “2 years of Ruby, 1 year of Python and 2 years of Java”, we might be concerned that the person doesn’t have the depth of experience we need. Although this reaction is natural, it’s misguided.

The person with the second CV could be a better developer on a C# project than your language expert, despite having little or no C# experience. Let’s not confuse them with a developer who happens to know a few languages. I’m talking about a particular kind of developer with varied experience and a good grasp of engineering fundamentals. The polyglot programmer.

**pol·y·glot**

adjective: knowing or using several languages

Source: [thoughtworks.com](https://www.thoughtworks.com/p2magazine/issue09/hire-polyglot/)

## Follow Dietzler’s Law
* 80% of what the user wants is fast and easy
* The next 10% is possible but difficult (and expensive)
* The last 10% is impossible

**But… users wants 100% of what they wants!**

## Prefer Libraries Over Frameworks
What is a difference between a framework and a library? The key difference is how you can use them and what kind of code you need to write.

Frameworks. When using a framework, the framework is in charge of running the system. It defines some extensibility points (interfaces) where you need to put your implementation.

Libraries. When using a library, you are in charge of running the system. The library defines some points through which you can access it (functions and types) and your code can call it as it needs.

Source: [tomasp.net](http://tomasp.net/blog/2015/library-frameworks/)

## Containers, not Virtual Machines
Containers include the application and all of its dependencies --but share the kernel with other containers, running as isolated processes in user space on the host operating system. Docker containers are not tied to any specific infrastructure: they run on any computer, on any infrastructure, and in any cloud.

## Pull Messages From Queues, Don't Push Them Out
