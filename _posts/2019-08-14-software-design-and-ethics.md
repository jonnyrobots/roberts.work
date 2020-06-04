---
layout: post
title:  "Design ethics and software design"
abstract: Ethically weak software is the outcome of the poor application of design.
date:   2019-08-14 13:45:59 +0000
readtime: 1 minute
categories: sabbatical article
--- 

# Design ethics and software design
### Where bad products come from 

Ethically weak software may be the outcome of deploying design to the wrong area of your product. My suspicion is that there’s a link between where companies choose to apply their design effort, and the growing number of stories about naughty software<a href="#1"><sup>1</sup></a>. 

As prevailing wisdom goes, you start with generalists before adding in specialists later. There’s a graph to illustrate this in “Intercom on starting up“: 

![Generalists:Specialists]({{ site.baseurl }}/images/intercom-specialists.jpg)

Assuming the right-most bar was representative of Intercom around the same time the book was published (2017), 75% of their (then) ~230 staff<a href="#2"><sup>2</sup></a> would be considered generalists.

Specialists have laser focus on one thing. If the majority of the design staff you employ when starting a company – or indeed a project – are specialists, then it stands to reason that you could end up with great execution on terrible ideas. 

Are the specialists aware of what they're contributing to? Maybe they are. Maybe they don’t care. Maybe they just [don’t realise](https://en.wikipedia.org/wiki/Hanlon%27s_razor). Systems are complex.

I asked a Software Engineer about a programme they were in charge of. This initiative involved at least 20 other humans and ran over 10 months each year. What I wanted to know was how *they* knew how it all hung together; “It’s in my head. It’s pretty simple.”.

We tested that assumption by setting aside 90 minutes (“do you think we’ll need that long?”) for them to draw me a [rich picture](https://en.wikipedia.org/wiki/Rich_picture). Two hours later they’d hit the edges of the paper, identified new connections and had seen the complexity that exists in even “simple” systems.

So what chance would you stand when designing the interface, for example, of a more complex system? How do you ensure that system is not damaging? Perhaps drawing a rich picture is a good start short-term. Then what? Redesign your design culture? Only employ [licensed designers](https://www.fastcompany.com/90161166/this-design-generation-has-failed)?

<hr/>

<a name="1"></a>
<sup>1. [Superhuman](https://www.theverge.com/2019/7/3/20681655/superhuman-email-app-spying-controversy-policy-change-read-receipts), [Volkswagen](https://en.wikipedia.org/wiki/Volkswagen_emissions_scandal), [Facebook](https://www.theguardian.com/technology/2019/mar/17/the-cambridge-analytica-scandal-changed-the-world-but-it-didnt-change-facebook)…
</sup>
<br/>
<a name="2"></a>
<sup>2. [Intercom to double Dublin base](https://www.irishtimes.com/business/technology/intercom-to-double-dublin-base-as-it-adds-350-jobs-worldwide-1.3408569)
</sup>
