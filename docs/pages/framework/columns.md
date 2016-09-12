---
title: Columns in The Framework
keywords: Columns
sidebar: framework_sidebar
permalink: columns.html
summary: An explanation of the different columns in The Framework
---

## LEVELS
See [levels](levels.md).

## CULTURE
**Organizational culture** encompasses values and behaviors that "contribute to the unique social and psychological environment of an organization." According to Needle (2004), organizational culture represents the collective values, beliefs and principles of organizational members and is a product of such factors as history, product, market, technology, strategy, type of employees, management style, and national culture; culture includes the organization's vision, values, norms, systems, symbols, language, assumptions, beliefs, and habits.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Organizational_culture)

### Further Reading
* [Organizational culture](https://en.wikipedia.org/wiki/Organizational_culture)

## BOUNDED CONTEXT
> Bounded Context is a central pattern in [Domain-Driven Design](https://en.wikipedia.org/wiki/Domain-driven_design). It is the focus of DDD's strategic design section which is all about dealing with large models and teams. DDD deals with large models by dividing them into different Bounded Contexts and being explicit about their interrelationships.

Source: [martinfowler.com](http://martinfowler.com/bliki/BoundedContext.html)

### What is the Domain Model?
> The Domain Model is the structured knowledge that is related to a specific problem. The Domain Model itself could be code, written prose or a diagram, the medium itself is not really important.

>The Domain Model focuses its attention on a specific problem. This constraint forces you to really get at the heart of the problem whilst ignoring everything from the outside world.

> This means that the Domain Model will have it’s own internal language that represents the important things that are specific to that one problem.

Source: [culttt.com](http://culttt.com/2014/11/19/bounded-contexts-context-maps-domain-driven-design/)

### What is a Bounded Context?
> A Bounded Context is the boundary that surrounds a particular model. This keeps the knowledge inside the boundary consistent whilst ignoring the noise from the outside world.

>This is beneficial for a number of reasons.

>Firstly you can model the aspects of the problem without having to be concerned with other parts of the business. Using the example from earlier, a Product object within the stock system only needs to be concerned with the methods and properties of that single system, rather than any other business concern that happens to fit on an object called Product.

>Secondly the terminology within a Bounded Context can have single, clear definition that accurately describe the problem at hand. Different departments across a company will usually have slightly different ideas and defin
itions of similar terms, but this can often derail a project through a lack of clarity and understanding when terms are mixed.

Source: [culttt.com](http://culttt.com/2014/11/19/bounded-contexts-context-maps-domain-driven-design/)

### What is a Context Map?
> When you start to think about the various subsystems of an application as individual Bounded Contexts, you can lose sight of the global view of the business as a whole.

> It is inevitable that the various Bounded Contexts of an application will need to communicate or share data between each other.

> A Context Map is the global view of the application as a whole. Each Bounded Context fits within the Context Map to show how they should communicate amongst each other and how data should be shared.

Source: [culttt.com](http://culttt.com/2014/11/19/bounded-contexts-context-maps-domain-driven-design/)

### Further Reading
* [What are Bounded Contexts and Context Maps in Domain Driven Design?](http://culttt.com/2014/11/19/bounded-contexts-context-maps-domain-driven-design/)
* [BoundedContext](http://martinfowler.com/bliki/BoundedContext.html)
* [What is the Domain Model in Domain Driven Design?](http://culttt.com/2014/11/12/domain-model-domain-driven-design)

## IT ARCHITECTURE
>  IT architecture is a series of principles, guidelines or rules used by an enterprise to direct the process of acquiring, building, modifying and interfacing IT resources throughout the enterprise. These resources can include equipment, software, communications, development methodologies, modeling tools and organizational structures.

Source: [Gartner](http://www.gartner.com/it-glossary/architecture/)

## BUILD
Coming soon

## SHIP
**Ship** (Software deployment) is all of the activities that make a software system available for use.

In continuous delivery, we introduce two new architectural attributes: testability and deployability.

In a testable architecture, we design our software such that most defects can (in principle, at least) be discovered by developers by running automated tests on their workstations. We shouldn’t need to depend on complex, integrated environments in order to do the majority of our acceptance and regression testing.

In a deployable architecture, deployments of a particular product or service can be performed independently and in a fully automated fashion, without the need for significant levels of orchestration. Deployable systems can typically be upgraded or reconfigured with zero or minimal downtime.

Source: [Continuousdelivery.com](https://continuousdelivery.com/implementing/architecture/)

### Further Reading
[Continuousdelivery.com](https://continuousdelivery.com/implementing/architecture/)

## RUN
Coming soon

## CHANGE
Coming soon
