---
layout: post
title:  "Reverse engineering CLI design"
abstract:  What makes a good CLI design
permalink: /articles/reverse-engineering-cli-design/
date:   2020-11-02 21:30:00 +0000
categories: article
readtime: 5 minutes
---

# Reverse engineering CLI design
### Understanding good design for the command-line

General wisdom says anyone using the command-line tool is a power user. I don't believe that's true. And even if it were, it’s no excuse for a poor developer experience. Creating a useful and widely-adopted developer tool requires consideration for its design. 

<a href="#a-reverse-engineered-guide-to-cli-design">Skip the context and tell me what makes a good CLI design</a>

I work on [Flyway](https://flywaydb.org), an OSS command-line tool for managing database migrations. I'm a Product Manager, but I come from product design. I'm always looking for ways to improve the design and experience of my product. 

Last week I caught [@jamonholmgren](https://twitter.com/jamonholmgren/status/1318738669243568128)’s Tweet about a nice CLI design update to [Ignite](https://github.com/infinitered/ignite), a tool for spinning up React Native apps. 

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I&#39;m rebuilding Ignite CLI, and this is when I wish my terminal design skills were better.<br><br>It&#39;s not bad. Definitely better than the old Ignite help screen. I just think I can do a lot better. <a href="https://t.co/nUHPrgfTDb">pic.twitter.com/nUHPrgfTDb</a></p>&mdash; Jamon Holmgren (@jamonholmgren) <a href="https://twitter.com/jamonholmgren/status/1318738669243568128?ref_src=twsrc%5Etfw">October 21, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

I thought the design looked strong. When I asked about design guides or resources used during development, Jamon's answer was none, and that “[there's basically nothing out there](https://twitter.com/jamonholmgren/status/1318957768640876546)”, which matches my experience[^1]. 

The fact that there's little help out there for designing non-GUI tools is a real shame.

So instead of continuing to search for the guide to the perfect CLI design, I’ll try to write it. Today I’m starting by reverse-engineering Jamon’s excellent design work 👆, then building a list of design principles from it for you to follow. 

Why go to the effort? Can’t you just copy this design? Yes and no. Most people can look at something and intuitively appreciate a good design. I can look at a painting of a horse and try to replicate it, but I'll get better results from learning how to draw one from first principles.

Reverse engineering a good design doesn’t just identify what’s good, but should help explain why it is good. Knowing this will help you replicate the outcome of the design for your product needs, and not just the tool you’re looking at verbatim.


### A reverse engineered guide to CLI design
#### How to use this guide

I’m going to structure this ‘reverse engineering of design’ by **user need**, phrased as a question a user would ask themselves, followed by an **illustration**, describing an example from the Ignite CLI.

When you’re using the guide, practice putting yourself in the shoes of your users and asking the same questions. The right way to answer each for _your product_ might be different.

One last thing, since I’m focussing on the CLI design for the moment, I’ve skipped ahead of the whole experience of finding the product in the first place, and indeed installing it. If this guide proves helpful, then [let me know](https://ctt.ac/lOd60) and I’ll follow up with some discovery and installation design guides.

Let’s go...

![Ignite CLI]({{ site.baseurl }}/images/ignite-cli.jpeg)

#### A. "Is this thing on?"

What we’re looking at in the screenshot above is a result of someone running the help command <span>`ignite --h`</span>. Providing the help option is command-line tool design 101, but it serves an interesting use case for a good developer experience (beyond the help itself):

When I run <span>`-h`</span> as a user, I’m getting two things: confirmation that the tool is installed correctly (without doing something destructive), and secondly, some idea of what to do next.

As a user I can also get the first effect – confirmation of install – by running <span>`-v`</span> – the command-line option that tells me what version of the tool I’m running – but encouraging users to run <span>`-h`</span> as the first step after install also provides hints as to what to do next, and without switching context and reading docs.

👉 Remember to reserve <span>`-h`<span> and <span>`-v`</span> for "help" and "version", and not to repurpose them as commands specific to your tool. 

#### B. "Am I in the right place?"

Ideally they've starting from your website and docs, but more likely they read about it on a blog describing a solution to the problem they just Googled.

I think Ignite does a really good job here of confirming I'm using the right thing. If the blog I read says "Install ignite" and the output of <span>`-h`</span> proudly proclaims "🔥 <span style="color: #dd0000">Ignite</span> 🔥", then I know I'm on the right path to solving my issue.

👉 Not all CLIs are created equal and not every CLIs will render emoji - something [Windows is terrible at](https://twitter.com/jamonholmgren/status/1318753153165053952) in general, and eerily reminiscent of browser/CSS standard compatibility (IE6 and rounded corners, anyone?).    

#### C. "Do I understand what this does?"

This might sound similar to the question above, but it's purpose is different and indicative of the difference between GUI and CLI. A GUI helps the user build a mental model of the system using a visual representation. CLI doesn't have that benefit, but requires the same outcome. 

Ignite achieves this with the information that "Ignite is a CLI that helps you spin up a new React Native app using a battle-tested tech stack". 

We can illustrate the mental model being built with this sentence by looking at the etymology of a couple of the phrases used:  

+ **[Spinup](https://en.wiktionary.org/wiki/spinup)**: (computing) The process of a disk drive spinning up.
+ **[Tech stack](https://en.wiktionary.org/wiki/stack)** In computing. A standard set of software components commonly used together on a system.

👉 I don't think it's feasible to rely on the command-line to impose a mental model on your user, particularly in more complex scenarios. At this point it's useful to defer to project documentation, with illustrations - something we do in [Flyway](https://flywaydb.org/documentation/getstarted/how). 


#### D. "Do I understand the implications of my actions?"

This question is about user trust. The CLI is often considered a more powerful interface because its assumption is that you know what you're doing. But that also makes it harder to gain trust - do I really want to copy-paste that <span>`sudo`</span> command I found on the internet without understanding what it will do?

Ignite achieves this by listing all the commands, with a description of their purpose and an example of its use, in a table. The design of the commands table in Ignite is good because it:

+ Lists commands in structured format that's easy to read as a **human**. 
+ Uses contrasting to differentiate command from description

👉 Whenever your command-line returns an output, think about the format of that content. Pure json – ie. a long string of text – might be machine readable, but it less easy for a human to parse. If a human needs to parse the output, make sure you structure it. 

#### E. "Now what?"

Understanding a handful of commands is just the beginning. Individual differences in technical environments and requirements make it near impossible to cater for every eventuality in the tool. That's where human help comes in - either through documentation or through asynchronous conversation.

Ignite does a great job of not just linking out to its documentation, but goes one step further by creating somewhere for its user community to go, and to support itself via their Slack community.

👉 The user "community" is a really powerful ecosystem for a lot of products, but especially so for developer tools. People get attached to their tools and like the affirmation of their good choices from like-minded people. Perhaps a better reason to create and support a community is for the opportunities to spot and improve on usability issues.   

### Summary

This is an all too brief review of one command-line tool. It's not intended to be a comprehensive guide to CLI design, but a first step towards a more complete guide to designing for the CLI, which you can register your interest in getting an early look at below:

<script async data-uid="de5ff9a08d" src="https://relentless-maker-3970.ck.page/de5ff9a08d/index.js"></script>

<hr/>

**Footnotes**

[^1]: The information that is out there is disparate, and is either too esoteric to be practical, or is practical but lacks substance