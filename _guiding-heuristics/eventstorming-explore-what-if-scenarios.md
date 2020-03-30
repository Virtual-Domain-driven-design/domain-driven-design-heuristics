---
title: "EventStorming: Explore what-if scenarios"
excerpt: "Explore all the edge cases and what happens when things go wrong."
tags: guiding-heuristics eventstorming
authors: Cédric Pontet
---

# Description

At the beginning of an EventStorming session, we tend to focus on the happy path, what happens when things go well and we reach the end of our process without an issue. But life is not that easy! We all know that sometimes things don't go according to the initial plan.

# Summary of the solution

After you figure out the nominal scenario, focus on other branches. What happens when this thing does not work? What if the API call to that *External System* fails? What if there is not enough money on the bank account?

Don't explore all branches at once, or you will get lost. Every time a new *what if* branch comes up, write it down as a Hot Spot (ping/magenta sticky) to keep track of it, then continue with the branch you are on. Once you are done exploring your branch, come back to the most interesting *what if* scenario and start exploring it. You might eventually decide that it is not worth exploring, but at least you know it exists.
