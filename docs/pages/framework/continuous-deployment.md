---
title: CONTINUOUS DEPLOYMENT
keywords: Continuous Deployment
sidebar: framework_sidebar
permalink: continuous-deployment.html
toc: true
summary:
---

## Defining Continuous Deployment
First of all, there's the somewhat pedantic fact that deployment does not imply release. As we say in the book, you can continuously deploy to UAT - no big deal. What makes continuous deployment special is deploying every change that passes the automated tests (and optionally a short QA gate) to production.

Source: [continuousdelivery.com](https://continuousdelivery.com/2010/08/continuous-delivery-vs-continuous-deployment/)

![Continuous Delivery vs Continuous Deployment](http://blog.crisp.se/wp-content/uploads/2013/02/continuous-delivery-deployment-sm.jpg)

Source: [crisp](http://blog.crisp.se/2013/02/05/yassalsundman/continuous-delivery-vs-continuous-deployment)

## Is It Worth the Time?
![Is It Worth the Time?](http://imgs.xkcd.com/comics/is_it_worth_the_time.png)

Source: [xkcd](http://xkcd.com/1205/)

## Deploying to Production != Release
Just because the code is deployed to production that does not necessarily mean that a new function is released. The recommended pattern for this are Feature Toggles.

### Feature Toggles
A feature toggle, (also feature switch, feature flag, feature flipper, conditional feature, etc.) is a technique in software development that attempts to provide an alternative to maintaining multiple source-code branches (known as feature branches).

Continuous release and continuous deployment provide developers with rapid feedback about their coding. This requires the integration of their code changes as early as possible. Feature branches introduce a bypass to this process. Feature toggles bring developers back to the track, but the execution paths of their features are still "dead" if a toggle is "off". But the effort is low to enable the new execution paths just by setting a toggle to "on".

The technique allows developers to release a version of a product that has unfinished features. These unfinished feature are hidden (toggled) so they do not appear in the user interface. This allows many small incremental versions of software to be delivered without the cost of constant branching and merging.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Feature_toggle)

## Justification Of The Choices Made
* The benefits of manual acceptance test does not outweigh the increased dependencies that build up in the staging environment and the effort involved in doing the manual tests

## The Other Alternatives That Were Not Chosen
* Continuous Delivery

## Further Reading
* [Continuous Delivery vs Continuous Deployment](https://continuousdelivery.com/2010/08/continuous-delivery-vs-continuous-deployment/)
* [Feature Toggles](http://martinfowler.com/articles/feature-toggles.html)
* [Continuous Deployment with Containers](https://www.infoq.com/articles/continuous-deployment-containers)
