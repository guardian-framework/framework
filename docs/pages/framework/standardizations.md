---
title: STANDARDIZATIONS
keywords:
sidebar: framework_sidebar
permalink: standardizations.html
toc: true
summary:
---

## **N.B. This page is [Opinionated](http://www.urbandictionary.com/define.php?term=Opinionated)!**
* There are clearly other choices that can be made
* The choices reflect our vision of what workings
* I you can make a strong case for making another choice, we would love that feedback via the link above

## Standardize ONLY when
* Deemed necessary for the sake of interoperability
* There is clearly a "better way of doing it"
* The cost involved is to high for be handled by each team

## REVISION CONTROL AND SOURCE CODE MANAGEMENT

### [GitHub](https://github.com)
> GitHub is a web-based Git repository hosting service. It offers all of the distributed revision control and source code management(SCM) functionality of Git as well as adding its own features. Unlike Git, which is strictly acommand-line tool, GitHub provides a Web-based graphical interface and desktop as well as mobile integration. It also provides access control and several collaboration features such as bug tracking, feature requests,task management, and wikis for every project.

Source: [Wikipedia](https://en.wikipedia.org/wiki/GitHub)

## BUG TRACKING, FEATURE REQUESTS, TASK MANAGEMENT AND DOCUMENTATION

### [GitHub](https://github.com)
> GitHub is a web-based Git repository hosting service. It offers all of the distributed revision control and source code management(SCM) functionality of Git as well as adding its own features. Unlike Git, which is strictly acommand-line tool, GitHub provides a Web-based graphical interface and desktop as well as mobile integration. It also provides access control and several collaboration features such as bug tracking, feature requests,task management, and wikis for every project.

Source: [Wikipedia](https://en.wikipedia.org/wiki/GitHub)

## CONTAINER TECHNOLOGY

### [DOCKER CONTAINERS](https://www.docker.com/what-docker)
Docker containers wrap a piece of software in a complete filesystem that contains everything needed to run: code, runtime, system tools, system libraries – anything that can be installed on a server. This guarantees that the software will always run the same, regardless of its environment.


## CONTAINER ORCHESTRATION

### [KUBERNETES](http://kubernetes.io/)
Kubernetes is an open-source system for automating deployment, scaling, and management of containerized applications.


## CAAS (CONTAINER AS A SERVICE

### [GOOGLE CONTAINER ENGINE](https://cloud.google.com/container-engine/)
Google Container Engine is a powerful cluster manager and orchestration system for running your Docker containers. Container Engine schedules your containers into the cluster and manages them automatically based on requirements you define (such as CPU and memory). It's built on the open source Kubernetes system, giving you the flexibility to take advantage of on-premises, hybrid, or public cloud infrastructure.


## CONTAINER WORKFLOW

### [DEIS WORKFLOW](https://deis.com/workflow/)
Deis Workflow is an open source Platform as a Service (PaaS) that adds a developer-friendly layer to any Kubernetes cluster, making it easy to deploy and manage applications.


## CONTAINER REGISTRY

### [GOOGLE CONTAINER REGISTRY](https://cloud.google.com/container-registry/)
Fast, private Docker image storage on Google Cloud Platform


## INTEGRATION BETWEEN SERVICES

### REQUEST-RESPONSE

#### RESTFUL: [JSON API](http://jsonapi.org/)
> If you’ve ever argued with your team about the way your JSON responses should be formatted, JSON API can be your anti-bikeshedding tool.

> By following shared conventions, you can increase productivity, take advantage of generalized tooling, and focus on what matters: your application.

> Clients built around JSON API are able to take advantage of its features around efficiently caching responses, sometimes eliminating network requests entirely.

#### RPC: [GRPC](http://www.grpc.io/)
A high performance, open source, general RPC framework that puts mobile and HTTP/2 first.

### PUBLISH-SUBSCRIBE

#### MESSAGING SYSTEM: [APACHE KAFKA](http://kafka.apache.org/)
Apache Kafka is publish-subscribe messaging rethought as a distributed commit log

#### INTERMEDIATE DATA FORMAT: [APACHE AVRO](https://avro.apache.org/docs/current/)
Apache Avro™ is a data serialization system.
Avro provides:
* Rich data structures
* A compact, fast, binary data format
* A container file, to store persistent data


## VERSIONING

### [SEMANTIC VERSIONING 2.0.0](http://semver.org/spec/v2.0.0.html)
> In systems with many dependencies, releasing new package versions can quickly become a nightmare. If the dependency specifications are too tight, you are in danger of version lock (the inability to upgrade a package without having to release new versions of every dependent package). If dependencies are specified too loosely, you will inevitably be bitten by version promiscuity (assuming compatibility with more future versions than is reasonable). Dependency hell is where you are when version lock and/or version promiscuity prevent you from easily and safely moving your project forward.

Given a version number MAJOR.MINOR.PATCH, increment the:
* MAJOR version when you make incompatible API changes,
* MINOR version when you add functionality in a backwards-compatible manner, and
* PATCH version when you make backwards-compatible bug fixes.

## ACCESSIBILITY

### [WEB CONTENT ACCESSIBILITY GUIDELINES (WCAG) 2.0](https://www.w3.org/TR/WCAG20/) - Level AA
> Web Content Accessibility Guidelines (WCAG) 2.0 covers a wide range of recommendations for making Web content more accessible. Following these guidelines will make content accessible to a wider range of people with disabilities, including blindness and low vision, deafness and hearing loss, learning disabilities, cognitive limitations, limited movement, speech disabilities, photosensitivity and combinations of these. Following these guidelines will also often make your Web content more usable to users in general.

## Search as a Service

### [ALGOLIA](https://www.algolia.com/)
> The Algolia model provides search as a service, offering web search across a client's website using an externally hosted search engine.

> Although in-site search has long been available from general web search providers such as Google, this is typically done as a subset of general web searching. The search engine crawls or spiders the web at large, including the client site, and then offers search features restricted to only that target site. This is a large and complex task, available only to large organisations at the scale of Google or Microsoft.

> Algolia's product only indexes their clients' sites and so the search task is far simpler. Data for the client site is pushed from the client to Algolia via a RESTful JSON API, then the search box is added simply to the client's web pages. This search model is intended to give the performance and sophistication advantages of a full in-house search engine operating on the native web site back-end database, but with the simplicity of setup of using a site-restricted Google search.

> Algolia claim a number of advantages for their approach, including speed of response from searching a single site rather than the entire web Moreover, as Algolia's search can be tailored to the client site, its known structure and its metadata facets, the search offered can be smarter and more site-specific than a generalised web text search. This improves the relevance of search results as searching may take the semantics of site content into account. A web site selling both puppies and dog clutches could avoid the search confusions and homonymy that bedevil the simple text-based search approaches.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Algolia)

## SECURITY

### [OWASP](https://www.owasp.org)
> The Open Web Application Security Project (OWASP) is an online community which creates freely-available articles, methodologies, documentation, tools, and technologies in the field of web application security.

Source: [Wikipedia](https://en.wikipedia.org/wiki/OWASP)

## Metrics and Alerting

### [Prometheus](https://prometheus.io/)
> Power your metrics and alerting with a leading
open-source monitoring solution.

## Distributed tracking

### [ZipKin](http://zipkin.io/)
> Zipkin is a distributed tracing system. It helps gather timing data needed to troubleshoot latency problems in microservice architectures. It manages both the collection and lookup of this data. Zipkin’s design is based on the Google Dapper paper.
