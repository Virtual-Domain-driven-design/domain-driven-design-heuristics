---
title: "Example Mapping: Write examples and formalise as intentions over implementation"
excerpt: "How can we remove the constraints of the current systen?"
tags: guiding-heuristics example-mapping behaviour-driven-development
authors: Kenny Baas-Schwegler
---

# Short description

When coming up with examples we want to let go of how the sytem is working now, and write down the intention as behaviour. For instance an implementation is:

```
Given no seats are reserved
When the user clicks on the reserve tickets button
Then the user should see the following seats reverved
```

 instead we want:

```
Given no seats are reserved
When we want to allocate seats
Then seats a9 - a11 will be reserved
```

At this stage I am not interested at all how we can automate it yet. Just that the example is clear.


# Context

When doing Behaviour-Driven Development we want to discover more knowledge and we can do that by using Example Mapping. During example mapping we start writing our examples for a specific business rule. A lot of examples explain the implementation of the system. For instance when a user clicks on button then. It can lead to all sort of coupling and being locked into the old system.