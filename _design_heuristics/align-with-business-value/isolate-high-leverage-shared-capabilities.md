---
layout: heuristic
---

# Isolate high-leverage shared capabilities

## short description

Create a shared bounded context that others bounded contexts in the company can use to avoid having to duplicate the logic in multiple contexts. Are there seperate concepts at play. Dependency management. Trading off dependencies. Local autonomy vs global consistency.

Don't create a shared dependency unless there is enough benefit. The benefit is that several teams reuse the shared capability which gives them more time to focus on their core areas.

### example

In a large enterprise several teams might use capabilities like notifications with for instance emailing or texting. 

## context

Use these at a strategic level when defining bounded context. When you want to seperate core domains from supporting and generic subdomains

## tags

## Author

Nick Tune