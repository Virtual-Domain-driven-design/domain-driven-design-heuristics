---
title: Align bounded context with the value stream
excerpt: "How do I design Bounded Contexts?"
tags: design-heuristics bounded-context socio-technical-systems
author: Marco Consolaro
---

# Short description

Align bounded contexts in socio-technical systems to support the value stream of the business. Use these at a strategic level when you are in a position to understand the value stream of the business.

# Examples
For example, in an ecommerce company selling physical items online, the value stream activities include:

* Acquiring (physically or remotely) the items to be sold 
* Describing their physical details (color, qualities, pictures and other information useful for their placement on the market)
* Assessing and interacting to handle the quantity in stock 
* Creating and managing the mechanism for customers to browse the catalogue, place an order and pay, dispatch the items

In parallel, there’s a marketing system to place advertisements, and after the sale is done, there will be some customer care functionality. This and all of the above are activities of the value stream. They can happen in parallel, and the stream might be somewhat complicated, but they can be carried on independently of one another. However, they have dependencies; for example, the system in charge of letting customers place an order obviously needs to know the stock of the available items – they are interconnected.

# Context

> _“If you can’t describe what you are doing as a process, you don’t know what you’re doing.”_ - William Edwards Deming

![Value stream](/assets/images/value-stream.png)

There is a vast amount of literature about value streams and value stream mapping, but I feel that the key concepts to understand aren’t enhanced with more detail. From this point of view, the idea of the Lean value stream as a diagrammatic representation of the sequence of activities that an organization undertakes in order to produce an overall result for a customer, stakeholder or end-user is the key starting point. 
The activities of the flow are independent, but interconnected; this is one of the properties of a Complex System. Each activity performs different tasks in autonomy, but feeds information back to other parts of the System that are needed for the chain of value to progress to the next stage.

In order to keep the overall entropy of the organization under control, the business must correctly separate and group these activities into independent but interconnected subsystems and optimize their communication. This is a crucial point. In the world of Domain-Driven Design, these subsystems are called _*bounded contexts.*_

![Value stream and bounded context](/assets/images/value-stream-contexts.png)

Since bounded contexts are high-level modules, there should also be among them a special focus on communication. Furthermore, given that to reach a good understanding we should move the focal point to the external system (as noted by Russell Ackoff), this explains why it is important to understand the value stream in order to design the best interaction flow between the bounded contexts. 

This logical, high-level view of the system is more important than the internals because it is the key to doing the right thing. And here the crucial point is finding the perfect balance between their independence and their interrelations, determining how to split them. What subtasks should be grouped together to form a bounded context, and what should be on their own?

![Bounded contexts and communication](/assets/images/value-stream-events.png)

The answer is that it depends on the overall context – there is no silver bullet here either, sorry! But we have principles that can help with the inductive process of making decisions. 
For instance, we can see here the same forces in place that we have seen in Cohesion and Coupling: 

* Too much Cohesion: Keeping every task in one big bounded context would mean entangling the system, making it hard to change and scale, similar to the God class and Divergent Change code smells. 
* Too much Coupling: Splitting every task into its own bounded context would mean moving that complexity over the communication between them, generating an explosion of dependencies. Furthermore, the way to achieving independence is not free in a SOA environment; the infrastructural boundary must be created, deployed, maintained and monitored. 

>_“You have to choose where to pay the price of complexity. Because DDD is about reducing complexity in the software, the outcome is that you pay a price with respect to maintaining duplicate models and possibly duplicate data.”_ - Eric Evans

![Bounded contexts and teams](/assets/images/bounded-context.png)
