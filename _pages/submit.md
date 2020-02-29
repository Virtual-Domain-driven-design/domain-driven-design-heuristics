---
title: About this website
layout: splash
permalink: /submit/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/kandinsky.jpg
---

# How it works

This sites works with jekyll trough a github repo linked with netlify. You can fork the github repo [here](https://github.com/Baasie/domain-driven-design-heuristics) and create a pull request of your own heuristics.

To work with Jekyll check out the [Jekyll Site](https://jekyllrb.com/)

# Adding your own heuristics

You can add your own heuristics as a markdown file under the respective _XXXX-heuristics directory. 

Not everyone uses github so alterntivly you can send your heuristic in an email to submit@dddheuristic.com.

# Writing, Remembering, and Sharing Design Heuristics

For more information please read about how to write Heuristics Rebecca her article [Writing, Remembering, and Sharing Design Heuristics](http://wirfs-brock.com/blog/2019/04/12/writing/)

There are some contraint when submitting a heuristic, you need to use at least the follow template:

## Template

``` markdown
---
title: {The title of the heuristic}
excerpt: {Summary of Problem or the question that the heuristic solves}
tags: {tags seperated by space, fill in what you think is best}
authors: {the authors seperated by comma}
submitter: {The submitter} (optional)
---

```

You can fill in the rest the way you like it, but here are two examples from Rebecca her article

### Quick Heuristic from QHE cards

``` markdown
---
title: {The title of the heuristic}
excerpt: {Summary of Problem or the question that the heuristic solves}
tags: {tags seperated by space, fill in what you think is best}
authors: {the authors seperated by comma}
submitter: {The submitter} (optional)
---

# Short description
A short description of the heuristics

# Examples
Give some examples

```

### From QHE card to a Heuristic gist:

``` markdown
---
title: {The title of the heuristic}
excerpt: {Summary of Problem or the question that the heuristic solves}
tags: {tags seperated by space, fill in what you think is best}
authors: {the authors seperated by comma}
submitter: {The submitter} (optional)
---

# Description
A description of the heuristics

# Summary of Solution
The solution of the heuristic 

```

# Contribute

Any help is welcome and needed, if you have any feedback please feel free to either create pull requests or tickets or send us an email!
