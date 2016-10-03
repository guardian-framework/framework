---
title: BUSINESS SERVICES
keywords: Business Services
sidebar: framework_sidebar
permalink: business-services.html
toc: false
summary:
---

## Conway’s law
> Any organization that designs a system (defined more broadly here than just information systems) will inevitably produce a design whose structure is a copy of the organization's communication structure.  
> <br>– Melvin Conway

## Defining Business Services
A business service is created to realize a business capability. The business capability (along with supporting capabilites and delimitations) form the purpose for the business service.

![Business Service formed around a business capability](images/business-service-capability.png)

<div>Icons made by <a href="http://www.flaticon.com/authors/gregor-cresnar" title="Gregor Cresnar">Gregor Cresnar</a> from <a href="http://www.flaticon.com" title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a></div>

<br>
Viewed from the outside, a business service has commitments to deliver services to it's customers based on the purpose. From a technology perspective most business services will offer digital services and/or conversion services (interfaces) for the customers to use in a self-service manner. Defined metrics (given to the service upon creation or revision) help the service to evaluate how it's performing and also for other services to see the progress.

Viewed from the inside the business service is operated be the business owner with the help of his/her cross-functional team, it's own technology (not shared with other services), information and processes.

![Business Service viewed from the inside](images/business-service.png)

## The business owner
The business owner is the only resource that is allocated to the service upon creation. The business owner shall have the vision and insight to guide the business service to success. The business owner is responsible for forming his/her autonomous team and together they will solve it's purpose with the help of technology, processes and the team itself.

## The "mother" of all (other) business services
As with the chicken or the egg causality dilemma first there has to be a egg that becomes a chicken that can lay other eggs. The first business service that has to be formed is the service that has the purpose of creating all other business services. This service is the only one that can create, change and remove business services.

![One business service to rule all other services](images/Business-service-for-services.png)

<div>Icons made by <a href="http://www.flaticon.com/authors/gregor-cresnar" title="Gregor Cresnar">Gregor Cresnar</a> from <a href="http://www.flaticon.com" title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a></div>

### Review process
Due the importance of the decisions made by this service, the review process is of the utmost importance. It's important to get different groups opinions before making a decision. The whole process should be made as public as possible to minimize any negative effect on other business services or the company as a whole.

## Template for establishing a business service
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#999;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#444;background-color:#F7FDFA;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#fff;background-color:#26ADE4;}
.tg .tg-ga2z{background-color:#f7fdfa;text-align:center}
.tg .tg-h8rl{font-weight:bold;color:#ffffff;text-align:center}
.tg .tg-bdj1{background-color:#d2e4fc;font-weight:bold;text-align:center}
.tg .tg-vr8s{font-weight:bold;background-color:#26ade4;color:#ffffff;text-align:center}
.tg .tg-iuhw{font-style:italic;background-color:#f7fdfa;text-align:center}
.tg .tg-w438{background-color:#d2e4fc;font-weight:bold;font-style:italic;text-align:center}
</style>
<table class="tg">
  <tr>
    <th class="tg-h8rl">Business Service Definition (Template)</th>
    <th class="tg-vr8s">Name:</th>
    <th class="tg-vr8s">Owner:</th>
    <th class="tg-vr8s">Version:</th>
  </tr>
  <tr>
    <td class="tg-bdj1">Purpose:</td>
    <td class="tg-bdj1">Rights:</td>
    <td class="tg-bdj1">Capability:</td>
    <td class="tg-bdj1">Governing Framework:</td>
  </tr>
  <tr>
    <td class="tg-ga2z">&lt;The purpose of the business service&gt;</td>
    <td class="tg-iuhw">&lt;What the business service has the right to do&gt;</td>
    <td class="tg-iuhw">&lt;The ONE capability that is the foundation for creating the business service&gt;</td>
    <td class="tg-iuhw">&lt;Which framework (e.g. GUARDIAN) should the business service adhere to&gt;</td>
  </tr>
  <tr>
    <td class="tg-w438">Commitments:</td>
    <td class="tg-bdj1">Delimitations:</td>
    <td class="tg-bdj1">Supporting Capabilities:</td>
    <td class="tg-bdj1">Metrics:</td>
  </tr>
  <tr>
    <td class="tg-ga2z">&lt;What the business service is required to deliver&gt;</td>
    <td class="tg-iuhw">&lt;What the business service is NOT allowed to do&gt;</td>
    <td class="tg-iuhw">&lt;Capabilities that are not the foundation for the business service but still is something the service should be able to handle&gt;</td>
    <td class="tg-iuhw">&lt;Key metrics for measuring the success of the business service&gt;</td>
  </tr>
</table>

## Microservices and the Inverse Conway Manoeuvre
N.B. James Lewis talks about business capabilities. GUARDIAN defines capabilites differently but exchange his use of the word capabilities for the word business service and everything is the same.

<iframe width="560" height="315" src="https://www.youtube.com/embed/uicjqeZO690" frameborder="0" allowfullscreen></iframe>

## Justification Of The Choices Made
We believe that giving people a clear (and small) purpose and the freedom to solve it in the way they view best is the only way to get outstanding customer value and efficiency.

## The Other Alternatives That Were Not Chosen
* Functional/hierarchical organization

## Further Reading
* [Industrialised Service Delivery Redux I](https://itblagger.wordpress.com/2008/07/)
* [Modeling Business Capabilities by Combining Services with Communication Patterns (2)](https://blogs.msdn.microsoft.com/asehmi/2007/06/24/modeling-business-capabilities-by-combining-services-with-communication-patterns-2/)
