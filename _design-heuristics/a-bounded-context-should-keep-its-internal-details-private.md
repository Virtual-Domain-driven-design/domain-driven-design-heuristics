---
title: A bounded context should keep its internal details private
excerpt: ""
tags: design-heuristics
author: Mathias Verraes
submitter: Kenny Baas-Schwegler
---

# Short description

If you are keeping monetary units in say 10 digits internally in a service, you would only pass out an amount in 2 digits precision because that’s all other consumers of the event would need

# Examples

# Context
