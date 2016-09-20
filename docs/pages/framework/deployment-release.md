---
title: DEPLOYMENT != RELEASE
keywords: deployment release
sidebar: framework_sidebar
permalink: deployment-release.html
toc: true
summary: Just because the code is deployed to production that does not necessarily mean that a new function is released.
---

## Defining Deployment != Release
Just because the code is deployed to production that does not necessarily mean that a new function is released. The recommended pattern for this are Feature Toggles.

### Feature Toggles
A feature toggle, (also feature switch, feature flag, feature flipper, conditional feature, etc.) is a technique in software development that attempts to provide an alternative to maintaining multiple source-code branches (known as feature branches).

Continuous release and continuous deployment provide developers with rapid feedback about their coding. This requires the integration of their code changes as early as possible. Feature branches introduce a bypass to this process. Feature toggles bring developers back to the track, but the execution paths of their features are still "dead" if a toggle is "off". But the effort is low to enable the new execution paths just by setting a toggle to "on".

The technique allows developers to release a version of a product that has unfinished features. These unfinished feature are hidden (toggled) so they do not appear in the user interface. This allows many small incremental versions of software to be delivered without the cost of constant branching and merging.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Feature_toggle)

## Justification Of The Choices Made


## The Other Alternatives That Were Not Chosen


## Further Reading
* [Four Principles of Low-Risk Software Releases](http://www.informit.com/articles/article.aspx?p=1833567&seqNum=2)
