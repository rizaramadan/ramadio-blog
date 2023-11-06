+++
title = 'Necessary Characteristic Microservice'
date = 2023-11-06T12:11:04+07:00
draft = false
+++
After years of experience with microservices, I've come to the conclusion that in order to avoid the most problematic issues in microservices:
1. Microservices should be large enough. Ideally, 2 or 3 microservices per team consisting of 10 members would be ideal.
1. Asynchronous communication between services should be the norm, while synchronous API calls should be minimized as much as possible.

# Why Macroservices
Like a spectrum, having a monolith for a large team and system requires certain practices to be in place. Often, it demands a significant amount of development investment. This includes high test automation coverage, up-to-date documentation, and an established coding convention. These are things that are crucial but rarely seen as urgent by the business.
On the other hand, having microservices that encompass very small or narrow domains per service necessitates a substantial infrastructural investment. This involves capabilities like canary deployment, automated deployment with rollbacks, and automatic dependency updates. Again, these are important elements that aren't always viewed as pressing by the business.
However, both monoliths and microservices have their merits. The ideal scenario might be something that combines the best of both worlds. This would fall under the category of microservices—since having just two services means we can't label it a monolith anymore—but they would be large enough that both infrastructural and development investments are minimized. Let's call this "macroservices." With macroservices, the exponential communication overhead from managing a monolith without the right development approaches can be reduced. Simultaneously, keeping the services sizable ensures we avoid the challenges that come from having too many diverse services without adequate infrastructural support.

# Why Async-First
Here's the revised version of your text:
Relying 100% on service-to-service API calls is a recipe for disaster; avoid it at all costs. A brief 10-minute search on the internet about the pitfalls of distributed monoliths will explain why. Essentially, it is just that—a distributed monolith.
Introducing asynchronous communication can reduce the tight coupling between services, minimizing the necessity for high availability of a service and decreasing the number of communications between teams. Picture the difficulty when a team tries to deploy an update to its service and, unexpectedly, another team encounters an issue in their service because of that very update. An Async-First communication approach, using events or message brokers, can mitigate these types of issues. Naturally, we can't entirely eliminate coupling, as doing so might cause more problems than benefits. Thus, the primary goal should be to ensure more than 50% of communication is asynchronous, and to proceed with caution beyond that.

# Necessary but Not Sufficient
Those two characteristics are necessary, but not sufficient, for us to assert that our approach to microservices is the right one. Other essential elements need to be in place. However, as a starting point, and on average, beginning with macroservices and an async-first approach might offer the best return on investment for most organizations.
