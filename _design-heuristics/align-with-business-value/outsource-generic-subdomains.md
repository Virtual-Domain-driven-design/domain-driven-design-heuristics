---
title: Outsource generic subdomains
tags: design heuristic
author: Nick Tune
type: subheuristic
---
# Question

Should we write software for generic subdomains ourself?

# Short description

Sometimes dependencies are so generic that you don't want to invest time in it and you can either buy them off the shelf or use a SaaS functionality.

You only oursource when there is enough competition in that market

# Examples

Payment providers like stripe, paypal etc.
Usermanagement, single sign-on like AWS or oath.com

# Context

Use these at a strategic level when defining bounded context. When you want to seperate core domains from supporting and generic subdomains
