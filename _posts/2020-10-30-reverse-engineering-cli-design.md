---
layout: post
title:  "Reverse engineering CLI design"
abstract:  What makes a good CLI design
date:   2020-10-30 11:00:00 +0000
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

I’m going to structure this ‘reverse engineering of design’ by **user need**, phrased as a question the user might be asking themselves, followed by an **illustration**, using an example from the Ignite CLI. 

When you’re using the guide, practice putting yourself in the shoes of your users and asking the same questions. The right way to answer each for _your product_ might be different.

One last thing, since I’m focussing on the CLI design for the moment, I’ve skipped ahead of the whole experience of finding the product in the first place, and indeed installing it. If this guide proves helpful, then [let me know](https://ctt.ac/lOd60) and I’ll follow up with some discovery and installation design guides.

Let’s go...

![Ignite CLI]({{ site.baseurl }}/images/ignite-cli.jpeg)

#### A. "Is this thing on?

The entire design we’re looking at is a result of someone running the help command <span>`ignite --h`</span>. Providing the help option is command-line tool design 101, but it serves an interesting use case for a good developer experience (beyond the help itself):

When I run <span>`-h`</span> as a user, I’m getting two things: confirmation that the tool is installed correctly (without doing something destructive), and secondly, some idea of what to do next.

Incidentally, as a user I can get the first effect running <span>`-v`</span> (the command-line option that tells me what version of the tool I’m running), but encouraging users to <span>`-h`</span> as the first step after install provides hints as to what to do next, without switching context and reading docs. 

<hr/>

**Footnotes**

[^1]: The information that is out there is disparate, and is either too esoteris to be practical, or is practical but lacks substance