---
title: "Design Bounded Contexts around EventStorming Policies"
excerpt: "How do we design a bounded context?"
tags: design-heuristics EventStorming
authors: Kenny Baas-Schwegler
---

# Short description

From a process or design level EventStorming, design your bounded contexts around the purple sticky called a policy.

# Examples

* When a domain experts mentions: When this event happens we will start the reservation process. We can add a policy that can be names: Reservation process policy
* Sometimes a policy is a long running process for instance a timer to cancel a reservation when the ustomer has not payed. You can design these within your bounded context instead of spanning between.

# Context

During process and design level EventStorming we want to design our bounded context. Since we usually take a customer journey or a product it can span multiple bounded contexts.