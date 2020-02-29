---
title: Keep your domain model decoupled from frameworks
excerpt: "How can I let my domain model be decoupled from technical complexity?"
tags: design-heuristics
author: Kenny Baas-Schwegler
---

# Short description

The domain model is the core of our bounded context. When we implement the domain model we want the ability to keep this consistent with our ubiqituous language. We want the ability to quicly refactor this to represent our mind-model of our domain model.

# Examples

In java and C# you see the use of ORM mapping like JPA and Entity Framework in our domain model. This can quickly lead high coupling with our database domain.

# Context

When we implement domain models we want to seperate the domain model from other layers to keep the domain clean. We sometimes see the use of frameworks like ORM mapping in the domain model for easier use. This can lead to high coupling between the domain model and the database model, which we don't want.