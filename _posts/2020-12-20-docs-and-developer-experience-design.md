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
### How to improve documentation usability

In this article:


<strong><a href="#why-is-documentation-important-again">Why is documentation important again?</a></strong>  
    1.1 <a href="#the-intuitive-gui">The intuitive GUI</a>   
        1.2 <a href="#the-rise-of-text-based-uis">The rise of text-based UIs</a>  
<strong><a href="#how-to-design-great-documentation">How to design great documentation</a></strong>  
    2.1 <a href="#information-architecture">Information Architecture</a>  
    2.2 <a href="#types of documentation">Types of documentation</a>  
    2.3 <a href="#commercial-considerations">Commercial considerations</a>  
    2.4 <a href="#deciding-where-to-start">Deciding where to start</a>  
<strong><a href="#useful-resources">Useful resources</a></strong>  
    3.1 <a href="#footnotes">Footnotes</a>
<hr/>

### Why is documentation important again?

#### The intuitive GUI

Nothing did more to expand the adoption of computers than the graphical-user interface (GUI). Simple visual metaphors (a file, the desktop, a document) provided a shortcut to learning how to interact with software.

GUIs by their nature immediately explain how a system works, negating the need for documentation. Designers of intuitive products saw their salaries rise, while technical authors were unceremoniously set aside. If it needed a manual, the product had failed.

Today the trend for GUI-first products has slowed, and GUI-less products are reversing the trend entirely. When the UI is text-based there is less 'affordance', and documentation finds itself back at the center of the user experience.

Without graphical metaphors to fall back on, designers of command-line interface (CLI) products, for example, have to work harder to help their users build a mental model of how to work their software. 

#### The rise of text-based UIs

The popularity of CLIs as the primary interface is growing rapidly, due in large part to the desire for efficiency. A business starting out today wouldn’t dream of building its own payments infrastructure. It’d choose to hook into Stripe.

Three engineering principles reflect this preference:

1. **Automation** - prevent wasting time on repetitive tasks
2. **Agnosticism** - choosing the right technology for the task 
3. **Composabilty** - unique combinations match unique needs 

As a consequence of this, the humble CLI (and API) has found itself at the centre of a battle for competitive advantage. Good UX design – or should I say Developer Experience Design? – is once again a differentiator. The easier your CLI is to use, the greater the chances your product is chosen over the competition.

Where CLI (and API, ML and AI) products were once the domain of deeply technical people, today that is demonstrably less true[^1]. The field of User Experience (UX), and Human Computer Interaction (HCI) – fields that arguably lead to the creation of the GUI – have some catching up to do. 

The ability to learn how to drive a CLI product relies heavily on good documentation across all levels of user competency. What makes for good documentation might seem obvious, but from my experience working on [@flywaydb](https://twitter.com/flywaydb), the task of producing it quickly becomes complex.

If UX wants to remain a valued role in the design and development of this category of product, then learning how to produce usable documentation is a good place to start.

## How to design great documentation

First, documentation needs to be designed to cater for four user scenarios:

1. Deciding whether this is the product I need
2. Trying out the product for the first time
3. Attempting to implement the product for real
4. Mastering the product

If you haven't yet spoken to your users in each of these modes, then this is top of your to do list. If you have, keep what you know close to hand as you make decisions in the following areas.

### Information Architecture

#### Finding things

It's important to think about how users end up on your documentation website, and specific documentation pages. There are generally just a handful of ways in which this happens: 

1. User saw your product referred to by name, and followed the link
2. User Googled the problem your product solves, and found your docs 
3. User hit a problem with your product in their environment

Think about how people arrive at the right piece of documentation.

If you're just starting out building your product, optimise your documentation for those scenarios in that order. 

For example, first offer help in forums and then document/link that help (point 1). Remember to use the same words and phrases as your users use to describe their problems, this'll help with SEO (point 2).

Help users who land on those pages understand where they are in the vast landscape of your documentation pages. 

[BREADCRUMB/MENU]

Now consider the more experienced users. Remind them that your docs exist with in-CLI links in error messages, and give them in-site search controls to help them locate specific documentation.

[SITESEARCHBAR]

#### Generic documentation Vs. Specific 

Agnosticism and composability, the engineering principles I referred to earlier, both conspire to erode the simplicity of your documentation.

Since there are multiple scenarios and environments in which modern  software products are used, there are multiple ways in which your product can acheive the same result. This flexibility is a gift and a curse.

Specific documentation is idiot-proof to follow, but generic documentation is flexible (and quicker to write).

One example of this in Flyway is API vs. CLI. Since our API is written in Java, developers writing software in other languages may choose to invoke Flyway from the command-line. Another example is configuration. Some users prefer to set configuration in a config file, and other prefer to pass the configuration via the command-line.

The ultimate goal is to have the user apply their parameters – details of their environment – to your documentation. 

[ProgrammingLanguage:Java,Configuration:Passviacommand-line.]

Since time and money aren't infite, pragmatism must obviously play a part. Refer back to the user scenarios above and start by writing opinionated and specific documentation for new user scenarios like "try it" guides, slowing moving to generic information as the topics you're documenting become more advanced. 

As you begin to increase your coverage of specifc documentation for different technical scenarios, use analytics data (like page visits) to determine the most popular environments to write specific document for first.   

####  Old stuff

Your product will evolve. New things will appear and old things will be deprecated. Semantic versioning (Ie. applying meaning to your version numbers) gives you options here.

The simplest choice is to replicate the entire documentation site at each major version release (Eg. in Flyway uses semantic versioning Major.Minor.Patch, eg. 7.5.3), asking the user up front what version of your product they want documentation for.

This covers the simplest scenarios, but inevitably there will be users who straddle two major version, and for them, a global feature to select which versions to show documentation for, or simple version tagging can be useful.

[SELECTOPTIONFORVERSION]

### Type of documentation

### Commercial considerations

### Deciding where to start


_Subscibe to the newsletter to be notified when the rest of the article – including how to make Information Architecture decisions, types of docs and what goes in them, and deciding how and where to start – is avaiable to read:_

<script async data-uid="378cd4c7af" src="https://relentless-maker-3970.ck.page/378cd4c7af/index.js"></script>

<hr/>

**Footnotes**

[^1]: This article – produced by a Product Manager with a background in User Experience – is written in Markdown, stored in a GitHub repository (<span>`git commit`</span> &gt; <span>`git push`</span> &gt; <span>`git merge`</span>) and compiled into the HTML you’re reading using Jekyll (<span>`jekyll serve`</span>). For free.