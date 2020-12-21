---
layout: post
title:  "Docs and Developer Experience Design"
abstract:  How to provide a good Developer Experience with documentation
permalink: /articles/docs-and-dev-experience-design/
date:   2020-12-20 21:30:00 +0000
categories: article
readtime: 5 minutes
---

# Docs &amp; Developer Experience Design
### Improving the Developer Experience with docs

Nothing has done more to expand the adoption of computers than the graphical-user interface (GUI). Simple visual metaphors (a file, the desktop, a document) provided a shortcut to learning how to interact with software. 

Point. Click. Done. 

GUIs, by their nature, explain almost immediately how a system works: “Click this button”. The same is not true for products where there is no GUI. 

Designers of command-line interface (CLI) products, for example, have to work harder to help their users build a mental model of how their software works.

The popularity of CLIs as the primary interface is growing rapidly. This growth is due in large part to an organisational desire to focus on its core competency. A software business starting out today wouldn’t build its own payments infrastructure, it’d use Stripe. 

Three engineering principles drive this trend:

1. **Automation** - prevent time waster on repetitive work  
2. Platform and Operating System (OS) **agnosticism** - prevent lock-in
3. **Composabilty** - enable unique needs to be met  

As a consequence of this, the humble CLI (and API) has found itself at the centre of a battle for competitive advantage. Good UX design – or should I say Developer Experience Design – is once again a differentiator. The easier our CLI is to use, the greater the likelihood of user adoption.

Where CLI (and API, ML and AI) products were once the sole domain of deeply technical people, that is demonstrably less true today[^1]. The field of User Experience (UX), and Human Computer Interaction (HCI) – fields that arguably lead to the creation of the GUI – have some catching up to do.  

The ability to pick up and learn a CLI product relies heavily on good documentation. Exactly what makes documentation *good* might seem obvious, yet from my experience working on [@flywaydb](https://twitter.com/flywaydb), the task of producing it quickly becomes complex.

To be continued...

_Subscibe to the newsletter to be notified when the rest of the article – including how to make Information Architecture decisions, types of docs and what goes in them, and deciding how and where to start – is avaiable to read:_

<script async data-uid="378cd4c7af" src="https://relentless-maker-3970.ck.page/378cd4c7af/index.js"></script>

<hr/>

**Footnotes**

[^1]: This article – produced by a Product Manager with a background in User Experience – is written in Markdown, stored in a GitHub repository (<span>`git commit`</span> &gt; <span>`git push`</span> &gt; <span>`git merge`</span>) and compiled into the HTML you’re reading using Jekyll (<span>`jekyll serve`</span>). For free.