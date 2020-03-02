---
layout: post
title:  "The evolution of theses"
subtitle: "No.002 Developing the core of a strategy"
date:   2020-02-09 20:45:59 +0000
categories: designance
---

# The evolution of theses
### No.002 Developing the core of a strategy

For this project to stand a chance of succeeding it ought to have a strategy. A good strategy requires a proven **thesis**, strong **principles** and according to [Rumelt](http://goodbadstrategy.com/about-the-book/), **coherent action**.  

My favourite strategy comes from one of the few firms to profit from the 2008 financial crisis. Their story is told by Michael Lewis in The Big Short [1]: 

> Their strategy was simple and brilliant... "People hate to think about bad things happening so they underestimate their likelihood."... 

It is simple, concise and easy to convey. I think it’s an excellent thesis. It also hints at insight.

> ...Jamie and Charlie found banks will sell options very cheaply on things they think will never ever happen. 

Cornwall Capital’s thesis, combined with this insight, formed the principles that enabled them act against conventional wisdom, and win:

> When they were wrong, they were wrong small. But when they were right, they were right big. Within a a few years they had turned their 110 grand into 30 million.

The importance of proven theses and strong principles hold true in software development. 

The most productive engineering teams I’ve worked with developed and tested their theses before writing a sinlge line of code. 

The principles you form following this process helps you achieve autonomy; the ability to make good decisions with good reason in good time. 

### Theses need time and experimentation

When I first discovered how to buy shares I faced a simple problem: who should I invest in? 

I discovered that fees for buying shares were around £11.95 per deal, putting a £100 investment 12% down the second it was purchased. 

Managed funds however, cost nothing to invest in and each fund listed its top ten investments anyway. I realised I could read this list and invest in the fund with the names of the companies I'd heard of and would have invested in anyway, for free [2]! 

`v0.1 - buy funds with the tech companies you know`

I bought shares in a technology fund at 190p and - over three and a half years – its value increased 39.5% until I sold them at 265p. 

This represents an average increase of 9.74% per year when, at the time, a basic savings account was paying out just 1.5% APR. So not bad, but actually some distance behind the sector average. 

This was a terrible investment thesis, but while it under performed it did return enough for me to risk buying company shares directly. And by now I’d developed a mechanism for choosing equities.

Companies hire intelligent people to make decisions about how to achieve company objectives. The objectives, which invariably revolve around the making of more money, often rest on software investments.

I believed that I was well positioned to decide which software company shares to buy, since I could see the difference each piece of software made to the success of the businesses I worked in [3], and simply copy those investments. Bringing me to my first thesis evolution: 

`v0.2 - buy shares in what the company invests in`

My results with this thesis were mixed. 

| Type A investment | Value | Type B investments | Value |
|-------|-------------|-----------|----------|
| Avalara  |   ⬇️3.6%  | Microsoft  |⬆️120.0%   |
| Zuora     |   ⬇️25%  | Salesforce  | ⬆️112%   | 

The first group, Type A, were investments made in companies whose software we purchased to facilitate some part of our business process. These are (so far) my least profitable investments.

The second group, Type B, are my most profitable and the insight I have here gets us closer to the thesis for Designance. 

Microsoft and Salesforce didn't just represent companies whose products we paid to use, but companies whose ecosystems we also invested engineering effort into. 

We worked closely with them, understood where their ecosystems fell short and wrote code that we turned into products to sell to our own customers.

Engineering teams are not cheap. The biggest I've been privileged enough to lead cost around $1m/yr. At the time it was focused on developing software for Microsoft's cloud platform, Azure. 

Developing for Azure gave us insight into Microsoft's strategy in the post-Balmer era; all in on Cloud. 

Microsoft saw that developers were choosing their (often open source) database technology according to a specific need – like CockroachDB for global scale-ability, Timescale for time-series data in IOT, Salesforce for customer relationship management [4] – and Cloud infrastructure for convenience. 

With Azure (and later its [$7.5 billion purchase of GitHub](https://techcrunch.com/2018/06/04/microsoft-has-acquired-github-for-7-5b-in-microsoft-stock/)), Microsoft has pitched itself squarely at developers. It no longer cares if you're using their proprietary technology, just that you’re building your application in Azure’s ecosystem.  

### Designing good software is getting harder

The Cloud, with its serious computing power and endless data storage provides easy access to automation. Combined with a lower barrier of entry to machine learning and artificial intelligence capabilities, the systems being built today are complex, difficult to comprehend and unsurprisingly, diffificult to design for.

The GUI - with its paradigms like buttons, check boxes and drop-downs - helped ordinary users develop a mental model for using a computer. They went on to help user experience designers contribute to the creation of valuable, intuitive software. 

Microsoft released its database engine nearly a decade after Oracle, but caught up quickly by providing a GUI on top. Now companies and their armies of software engineers seek automation, and guess what? The GUI doesn’t automate. 

In London, Facebook has a designer-to-developer ratio of 1:50 (5). While designers were distracted by creating the easy-to-open packaging, developers got on with designing the product; algorithms designed to hold your engagemtns, but that ended up delivering anxiety-inducing content that makes you angry and compelled to take another drag. It is digital cancer.

You can’t blame the designers for being stuck at the GUI level when it’s significantly easier to design an intuitive iPhone app than an algorithm that can’t be weaponized. For the moment.

`v0.3 - complex systems need specialist design tools`

There's been a proliferation in the creation of (graphical) design tools over the past decade – Invision, Sketch, Figma, Principal – but few, if any, go deeper than interface and interaction design.

More importantly not a single one has IPO'd, making Adobe the only creator of design tools that I can invest in right now. I think there's a gap here that I could explore with Designance.

All I need now is to make some decisions, and for that I'll need some principles.

![]({{ site.baseurl }}/images/sig.png)

<hr/>

**Footnotes**

+ [1] This is actually a line from the film. I chose to quote this since it's a more succinct evaluation of Cornwall Capital's investment strategy, which of you’re intrigued learn more, is described over several pages in the book from Chapter 5 - Accidental capitalists.
+ [2] It's important to point out that while there are no fees upfront, there is still no such thing as a free lunch and the cost is just hidden. This was as true for managed funds then as it is for fee-free share dealing now.
+ [3] This is what a stock picker in an active fund is paid to do; analyse and pick companies to invest in. This is in contrast to a passive fund, which invests in everything in a given sector. The difference is interesting at the moment since genius investors picking stocks for active funds are struggling to justify their existence by out-performing (cheaper) passive funds. 
+ [4] Salesforce is in essence just another database - albeit not one available on any Cloud platform other than Salesforce itself. Although I wasn’t involved with this project, developing software for the Salesforce ecosystem provided fantastic ROI, creating not just a new product,  but an entirely new company.
+ [5] In 2016 I went with a few of our design team to meet some of the designers at Facebook in London. I was given this ratio by a designer based on the teams they knew about, so this figure is anecdotal and probably out-of-date.