---
layout: post
title:  "The evolution of theses"
subtitle: "No.002 Developing the core of a strategy"
date:   2020-02-09 20:45:59 +0000
categories: designance
image: <img src="/images/thesis.png"/> 
---

![Developing a thesis]({{ site.baseurl }}/images/thesis.png)

**Preface**

I finished writing this post on 9th February 2020. Before I was ready to hit ‘publish’ the world changed, along with my plans for this project.

It used to take a year or two for me to recognise naivety, now it’s evident in days. And it’ll show in this like nothing I’ve written before. For example, it’s now clear that I’ve worked the majority of my career in a bull market.

Regardless, I decided to hit publish and deliver it to your inbox because I still believe there is something to be learned from exploring the premise that this project is based on.

--- 

*☕️ 15 minute read*

## Developing a thesis

A good strategy requires a proven **thesis**, strong **principles** and according to [Rumelt](http://goodbadstrategy.com/about-the-book/), **coherent action**. For this project to stand a chance of succeeding it ought to have a strategy. But where to start?

My favourite strategy story comes from one of the few firms to profit from the 2008 financial crisis, and it’s told by Michael Lewis in The Big Short <sup><a href="#footnotes">[1]</a></sup>:

> Their strategy was simple and brilliant… “People hate to think about bad things happening so they underestimate their likelihood.”…

I like it because it is simple, coherent and easy to remember.

> …Jamie and Charlie found banks will sell options very cheaply on things they think will never ever happen.

The thesis, combined with this insight, formed the principles that enabled Cornwall Capital to act against conventional wisdom, and win:

> When they were wrong, they were wrong small. But when they were right, they were right big. Within a few years they had turned their 110 grand into 30 million.

The importance of proven theses and strong principles hold true in software development too. The most productive engineering teams I’ve worked with developed and tested their theses before writing a single line of code.

The principles formed through the discipline of developing your thesis first, pay you back later with the ability to make good decisions with good reason in good time. In software development this state of nirvana is called autonomy.

## Time and experimentation

When I first discovered how to buy shares I faced a simple problem: who should I invest in?

I discovered that fees for buying shares were around £11.95 per deal, putting a £100 investment 12% down the second it was purchased.

Managed funds however, cost nothing to invest in and each fund listed its top ten investments anyway. I realised I could read this list and invest in the fund with the names of the companies I’d heard of and would have invested in anyway, for free <sup><a href="#footnotes">[2]</a></sup>!

`Thesis v0.1 - buy funds with the tech companies you know`

I bought shares in a technology fund at 190p and - over three and a half years – its value increased 39.5% until I sold them at 265p.

This represents an average increase of 9.74% per year when, at the time, a basic savings account was paying out just 1.5% APR. So not terrible, but some distance behind the sector average.

Despite being a (relatively) terrible investment thesis, under performing as it did, it did return enough for me to now risk buying company shares directly. And by then I’d developed a mechanism for choosing stocks.

Companies hire intelligent people to make decisions about how to achieve company objectives. The objectives, which invariably revolve around the making of more money, often rest on software investments.

I believed that I was well positioned to decide which software company shares to buy, since I could see the difference each piece of software made to the success of the businesses I worked in <sup><a href="#footnotes">[3]</a></sup>. This thesis was simple; copy these investments. Bringing me to my first thesis evolution:

`Thesis v0.2 - buy shares in whatever my employer invests in`

My results with this thesis were mixed.

**Type ‘A’ investments**

Avalara - 📉-3.6%, Zuora- 📉 -25%, …

**Type ‘B’ investments**

Microsoft 📈 +120.0%, Salesforce 📈+112%, …

The first group, Type A, were investments made in companies whose software was purchased to facilitate some part of the business process. These are (so far) my least profitable investments.

The second group, Type B, are my most profitable and the insight I have here gets us closer to the thesis for Designance.

Microsoft and Salesforce didn’t just represent companies whose products we paid to use, but companies whose ecosystems we also invested engineering effort into.

We worked closely with them, understood where their ecosystems fell short and wrote code that we turned into products to sell to our own customers.

Developing for Azure gave us insight into Microsoft’s strategy in the post-Balmer era; embrace open-source, add [support for Linux](https://www.wired.com/2016/06/microsofts-open-source-love-affair-reaches-new-heights/) and relax focus on proprietary software.

Microsoft saw that developers were choosing their (often open source) database technology according to a specific need – like CockroachDB for global scale-ability, Timescale for time-series data in IOT, Salesforce for customer relationship management <sup><a href="#footnotes">[4]</a></sup> – and Cloud infrastructure for convenience.

With Azure (and later its [$7.5 billion purchase of GitHub](https://techcrunch.com/2018/06/04/microsoft-has-acquired-github-for-7-5b-in-microsoft-stock/)), Microsoft has pitched itself squarely at developers. It no longer cared if you’re using their proprietary technology, just that you’re building your application in Azure’s ecosystem.

Engineering teams are not cheap. The biggest I’ve been privileged enough to lead cost (I’m told) around $1m/yr, so dedicating just one team to this endeavour represented a significant bet. This particular bet led me to my next insight.

## Designing good software is getting harder

The GUI - with its paradigms like buttons, checkboxes and drop-downs - helped ordinary people develop the mental model required for using a computer. They went on to help user experience designers contribute to the creation of valuable, intuitive software. Importantly, for anyone designing a product through the GUI provided a clear mental model of how the system was working.

Microsoft released its database engine nearly a decade after Oracle, but caught up quickly by providing a GUI on top. Now companies and their armies of software engineers seek automation, and guess what? The GUI doesn’t automate.

The Cloud, with its serious computing power and endless data storage provides easy access to automation. Combined with a lower barrier of entry to machine learning and artificial intelligence capabilities, means the systems being built today are complex, difficult to comprehend and remarkably difficult to design for.

Right now I’m working on a product designed for automation. Its human interface is a config file and command-line (or API) designed and developed by software engineers. For the majority of the time it’s in use, it’s being instructed by computers executing code written by other software engineers.

Learning to design this kind of product has been a challenge in which none of the design software I’ve used previously has been of any help.

Google – perhaps the most well-known provider of AI and ML-driven experiences – has 300 <sup><a href="#footnotes">[5]</a></sup> people working on its Design System, [Material](https://material.io/design/). That's the equivalent of a small-to-medium enterprise dedicated to helping humans interact with computers. Even so, when it comes to providing guidance on the design of AI and ML systems themselves, Material is still stuck [describing the superficial](https://material.io/collections/machine-learning/object-detection-live-camera.html#usage) layers of visual and interaction design.

In London, Facebook has a designer-to-developer ratio of 1:50 <sup><a href="#footnotes">[6]</a></sup>. Staff there still put out frequent Medium articles laying claim to their powers of visual design. Most of these posts come from “self-taught” Product Designers incapable of addressing the irony that the real product design is being carried out by the data “scientists” (furiously mining data) and software engineers (blindly writing algorithms that negatively impact the lives of their users).

For designers and users, the stakes have never been higher. Which brings me to:

`Thesis v0.3 - complex systems need specialist design tools`

There has been a proliferation in the creation of (graphical) design tools over the past decade – InVision, Sketch, Figma, Principal – but few <sup><a href="#footnotes">[7]</a></sup>, if any, go deeper than interface and interaction design.

Moreover, not a single one has IPO’d. Adobe is the only company making tools for designers of software products that I can invest in right now.

I think there’s a gap here that I could explore with Designance.

All I need now is to make some decisions, and for that I’ll need some principles.

![]({{ site.baseurl }}/images/sig.png)
<a name="footnotes"></a>

<iframe src="https://designance.substack.com/embed" width="480" height="320" style="border:1px solid #EEE; background:white;" frameborder="0" scrolling="no"></iframe>

**Footnotes**

+ [1] This is actually a line from the film. I chose to quote this since it’s a more succinct evaluation of Cornwall Capital’s investment strategy, which of you’re intrigued learn more, is described over several pages in the book from Chapter 5 - Accidental capitalists.
+ [2] It’s important to point out that while there are no fees upfront, there is still no such thing as a free lunch and the cost is just hidden. This was as true for managed funds then as it is for fee-free share dealing now.
+ [3] This is what a stock picker in an active fund is paid to do; analyse and pick companies to invest in. This is in contrast to a passive fund, which invests in everything in a given sector. The difference is interesting at the moment since genius investors picking stocks for active funds are struggling to justify their existence by out-performing (cheaper) passive funds.
+ [4] Salesforce is in essence just another database - albeit not one available on any Cloud platform other than Salesforce itself. Although I wasn’t involved with this project, developing software for the Salesforce ecosystem provided fantastic ROI, creating not just a new product, but an entirely new company.
+ [5] Stats taken from the Q&A section of a talk given by Elizabeth Churchill, Director of UX, Google Material Design in May 2019.
+ [6] I was given this ratio by a Facebook designer in 2016. It was based on the teams they knew about, so this figure is anecdotal and likely out-of-date.
+ [7] I say “few” because Roam - a “note-taking tool for networked thought” might, but it doesn’t appear to pitch itself at designers of software products and it is a steep learning curve to mastering it.

