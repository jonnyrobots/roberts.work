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

Coming up:
1. <a href="">Why is documentation critical again?</a>
   i. 
2. <a href="">How to design great documentation</a>

<hr/>

### Why is documentation critical again?

Nothing did more to expand the adoption of computers than the graphical-user interface (GUI). Simple visual metaphors (a file, the desktop, a document) provided a shortcut to learning how to interact with software.

GUIs by their nature immediately explain how a system works, negating the need for documentation. Designers of intuitive products saw their salaries rise, while technical authors were unceremoniously set aside. If it needed a manual, the product had failed.

Today the trend for GUI-first products has slowed, and GUI-less products are reversing the trend entirely. When the UI is text-based there is less 'affordance', and documentation finds itself back at the center of the user experience.

Without graphical metaphors to fall back on, designers of command-line interface (CLI) products, for example, have to work harder to help their users build a mental model of how to work their software. 

The popularity of CLIs as the primary interface is growing rapidly. This growth is due in large part to the desire for efficiency. A business starting out today wouldn’t dream of building its own payments infrastructure. It’d use Stripe. 

This trend is illustrated in three engineering principles:

1. **Automation** - prevent time wasted on repetitive work  
2. **Agnosticism** towards Platform and Operating System (OS) - prevent lock-in
3. **Composabilty** - enable unique needs to be met  

As a consequence of this, the humble CLI (and API) has found itself at the centre of a battle for competitive advantage. Good UX design – or should I say Developer Experience Design – is once again a differentiator. The easier your CLI is to use, the greater the chances your product is chosen over the competition.

Where CLI (and API, ML and AI) products were once the domain of deeply technical people, today that is demonstrably less true[^1]. The field of User Experience (UX), and Human Computer Interaction (HCI) – fields that arguably lead to the creation of the GUI – have some catching up to do. 

The ability to learn how to drive a CLI product relies heavily on good documentation across all levels of user competency. What makes for good documentation might seem obvious, but from my experience working on [@flywaydb](https://twitter.com/flywaydb), the task of producing it quickly becomes complex.

## How to design great documentation



_Subscibe to the newsletter to be notified when the rest of the article – including how to make Information Architecture decisions, types of docs and what goes in them, and deciding how and where to start – is avaiable to read:_

<script async data-uid="378cd4c7af" src="https://relentless-maker-3970.ck.page/378cd4c7af/index.js"></script>

<hr/>

**Footnotes**

[^1]: This article – produced by a Product Manager with a background in User Experience – is written in Markdown, stored in a GitHub repository (<span>`git commit`</span> &gt; <span>`git push`</span> &gt; <span>`git merge`</span>) and compiled into the HTML you’re reading using Jekyll (<span>`jekyll serve`</span>). For free.