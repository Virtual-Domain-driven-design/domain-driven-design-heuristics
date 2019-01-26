---
title: Don't use a framework in your domain model
tags: design heuristic
author: Kenny Baas-Schwegler
---

# Short description

The implementation of the domain model should not use any framework. 

# Examples

# Context

When we implement domain models with hexagonal or clean architecture we need to seperate the domain model from other layers to keep the domain clean. We sometimes see the use of frameworks like ORM mapping in the domain model for easier use. This can lead to high coupling between the domain model and the database model, which we don't want.