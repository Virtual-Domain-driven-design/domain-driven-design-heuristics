---
title: Design for replayability
excerpt: ""
tags: design-heuristic
authors: Nick Tune & Kacper Gunia
---

# Short description

Design projections so that they can be easily replayed per stream or projection type.

# Examples

A particular read model requires a new field that wasn't captured previously. Changing the logic and replaying it will make the field available for already existing read models as well as for newly created ones.

# context

In Event-Driven architectures and particularly in Event-Sourcing + CQRS the "read" part of the system is a projection of the Event Stream. Design the infrastructure of the event delivery to projection handler so that it can be easily replayed when bugs are discovered or requirements changed. It is usually a good idea to be able to replay either subset of streams or all of them.