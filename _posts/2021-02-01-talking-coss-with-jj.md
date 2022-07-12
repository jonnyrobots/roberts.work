---
layout: post
title:  "Capturing value as a COSS business"
abstract:  A conversation with Joseph Jacks (OSS Captial) about the challenges of capturing value as a commercial open source business.
permalink: /articles/coss-challenges/
date:   2021-02-01 21:30:00 +0000
categories: Article
readtime: 15 minutes
---

# Capturing value as a COSS business
### A conversation with Joseph Jacks, OSS Capital

Feel free to [⏩ skip to the conversation](#content), [🎧 listen to the audio version instead](#) or [⚡️ cheat altogether with the hightlights](https://twitter.com/jonny_robots/status/1356290000443289602) 

#### First, some background

For the last 6 months I've been scratching my head trying to solve a marketing challenge with [@flywaydb](https://www.twitter.com/FlywayDB) - how to increase our engagement and understanding of Flyway's userbase.

Flyway is Open Source software that's used by a lot of people and in a lot of organisations. It's been adopted by the central banks of many states, it's in use at technology companies, at retail and investment financial institutions, and at insurance companies and healthcare providers. 

That level of adoption is driven by the fact that Flyway is a strong, valuable and reliable product with its distribution having been accelerated on account of it being available as open source software. 

The flip side of easy distribution (oss) and adoption (it's free, the source code can be security reviewed) is poor visibility of who's using it. This is a real challenge when it comes to letting those users know when there's additional value to be had in the paid-for edition - especially for commercial organisations who rely on this code existing.

[Joseph Jacks](https://oss.capital/#team) – JJ – is someone who's been here before, and is so into Commercial Open Source software (COSS) he founded a VC firm with COSS at the centre of its investment thesis. I asked JJ to share his thoughts on this challenge, and to speculate on how a the person responsible for the commercial success of a COSS business might solve that today.

These are my notes from that conversation.
<a name="content"></a>

![COSS chat with JJ]({{ site.baseurl }}/images/coss-chat.png)

**I guess we should start with how we got to talking...**

> JJ: You responded to one of my Twitter threads on my early sales days at Talend and you said 'I want you to expand on that' and 'please blog about this', and I don't have time to blog about it these days, so we set up this meeting, and here we are.

That's it. The thread that caught my attention was about the challenges you faced back in the early 2010's, working in sales at Talend. I wasn't originally familiar with Talend, but I believe it's a company that started out life as an open source product. 

It seems Talend had good growth in adoption, and they'd succeeded in being able to reach their user base, and had this conversion funnel in place that's got them to a market cap of $1.39Bn today. 

**Can we get into a bit more detail about that today?**

> JJ: Yeah, happy to dig into that.

One of the stats that impressed me was that Talend were seeing around [10 to 15 thousand leads a generated each month](https://twitter.com/asynchio/status/1352873277677428737). If you're sitting in a sales position, knowing you have this massive group of users on the free open source edition AND you have their details, what a great position to be in.

I think a lot of people will be thinking 'just how did Talend get there?'. You attributed that volume to product telemetry and lead collection - from every user of the free, open source addition. 

So two things stick out to me there - the first is the challenge of gaining the trust of the free open source software users to add that telemetry, and the willingness to provide you with their details.

The second is the company had the commercial need to collect that data, **how did it balance that with it being a product that's embedded in the infrastructure layer, and all the technical constraints that we know go with that?**

> JJ: The balance that companies have to achieve when creating value and capturing value complex, [is true] regardless whether they're Open Source at the core, or freemium. <br/><br/>
> Digging into open-core and commercial Open Source companies, the biggest challenge that I've noticed is companies having a full observational reach into the users of their software and technology.<br/><br/>
> When you open source something there's this fundamental thing that happens when you apply an extremely permissive license to your source code. <br/><br/>
> What I've noticed is that the understanding and ability to track and know how many people are using your software, and how they're using your software and how it's performing for them, and what system is it touches - it's almost impossible to understand, or even infer.

**Why does that challenge exist, do you think?**

> JJ: This pseudonymous – or fully anonymous, in some cases – dynamic with open source, where you put something out onto the internet, you apply a permissive license to it, and there could be a huge number of people getting a ton of value from your software that you don't even know about, you don't even know they exist. <br/><br/>
> The vast majority of people using your software and getting value from it are invisible to you. You don't even know they're out there. But, they could be getting a ton of value, they can be evangelising to other people. You can have this invisible virality phenomena occurring. <br/><br/>
> In terms of just your energy in creating some piece of software, and the impact to the world, is unconstrained through this open source model. You have a massively compounding effect of value creation. This is really, really amazing on one hand for positive sum abundance in the world. On the other hand, as a software company founder, and a capitalist, it's very frustrating.

**Where do you start with trying to solve that?** 

> JJ: You have to really think about how to solve the problem of connectivity. From creating something that's really, really valuable for the world, putting it out there, but then also having a sense of [whether it's] possible for us to have an understanding of who's using our software and when. And is it possible to understand what people are doing with the software so precisely? How the software is being used? And what configurations? And and what integrations? And so on. <br/><br/>
> With open source, the last 15-20 years are very clearly concentrated in this infrastructure layer of the technology stack, where you've got a lot of integrations happening. 

**I guess that adds to the complexity?**

> JJ: You've got databases touching things, and other applications that want to reach into something, and systems of record that are very crucial to databases, and middleware that moves data one system to the other and does transformation, or maybe you've got something that's more like glue [like] API synchronisation, or network proxying. <br/><br/> 
> So those systems are even more pernicious in understanding the impact of the software. 

**What kind of things make this hard? And what kind of telemetry should we reasonably expect to be suitable for open source software prodcuts, and especially those working in this infrastructure layer?**
> I've thought a lot about that and I feel like – just to hypothesize – we're entering a new era where the Open Source movement is trying to adopt a lot of the  best practices from SaaS where you've huge amounts of data, and huge amounts of instrumentation from your users, but from the very beginning, as opposed to later on. <br/><br/>
> There's two phenomenon here. Let's just say nothing changes around where code is hosted and where the software is run. In that world, open source software is hosted primarily on on Github. Then people pull it down from GitHub, or from some package manager registry. <br/><br/> 
> Then you've got a company that forms around the project and they raise some venture capital and everybody's on a payroll, working really hard. Every VC under the sun is is investing in this category now. No one was doing it two years ago when we got started as a fund. 
> Now [January 2021] is the first month in history where we've reached 600 million in funding for COSS companies – commercial Open Source companies – just in a single month and that does not include this $2 billion round that Databricks is closing right now.

**Do you think when it comes to commercialising this software - and justifying these kinds of numbers, that these companies are going to be able to do that?**

> A large number of commercial product companies formed to create a consistent revenue stream, and hire more people, and create a market, or disrupt the market somehow. <br/><br/>
> They face this conundrum; do we continue to create open source that we cannot track? Or do we build commercial product and does the company only focus on proprietary IP that is really easy to track?  This balancing act is definitely a big question.<br/><br/> 
> This traditional way of thinking about funnel theory, [and] the stages of a marketing funnel: lead, to lead-qualified in some pipeline, and then advance to the sales process, and then close someone, and onboard them as a customer.<br/><br/>
> How that worked at Talend, [the way] Talend was able to collect information about the Open Source users was very different from, a decade later, how commercial Open Source companies collect data and understand their users. Vastly different.

**How would you describe how a modern COSS company does that today? How's that's different to Talend 10 years ago?** 

> JJ: I think the biggest thing that's different is GitHub did not exist a decade ago and it exists now. Not only does it exist now, it is this massive phenomena that powers software creation and collaboration on earth I think 50 million plus people are on GitHub now. A material fraction of that are active Open Source maintainers, creators and so on. <br/><br/>
> What I think was interesting about Talend in the absence of GitHub a decade ago, 2010, 2011, was that Talend maintained full control of where their Open Source was hosted, and where users discovered the software, how they discovered it, how they downloaded it, how they accessed it, how they learned about new updates and new changes and new interaction mechanisms, how they collaborated with providing feedback on issues and bugs and plugins.<br/><br/>
> If you really think about all of this, all of those things today they pretty much occur on one property; GitHub.<br/><br/>
> This is a huge change from the first wave of COSS companies, that took few people by surprise when you saw things like SpringSource or ZenSource or JBoss or Talend, or Magento or pick your example of really early mid-2000s – 2005, 2006 – to mid-2010's Commercial Open Source success stories.
> What I'm noticing in the last five years, really, in particular, a very short period of time, is the default choice a lot of commercial Open Source founders are making of where the software lives – and where all this metadata and collaboration, interaction and feedback exists – is on GitHub.

**What's your sense for what's going on at Microsoft/GitHub at the moment?**

> JJ: Microsoft is very gradually integrating GitHub into many of their offerings. Whether it's Visual Studio Code or Azure, all these other other platform tools. I don't think any of that is bad at all I think that's a really great progression for GitHub.<br/><br/> 
> I think GitHub will be 100 billion dollar asset within the next year or two for Microsoft.<br/><br/> 
> These network effects are really amazing, but I think the downside – and I'm trying to not be critical and dismissive of GitHub as the default safe choice for commercial Open Source founders to host their software – [is that project creators] give all of this data to another platform that they don't control. They should really be cognizant of the trade-offs.

That's an interesting observation about Github, that as a founder you get great distribution and network effects upfront, but at the cost of understanding your users and how they use your software. It's something that I hadn't considered before. 

In the last couple years GitHub started to raise the idea of value capturing features – like the ability to sponsor a project, for example – which would be a way of sustaining an Open Source project. 

**Do you think Microsoft/GitHub will go further than that?** 

> JJ: I think they will, it's a natural thing for them to explore. I think the sponsors technology and donations / Patreon-like workflow on Github is a great option. I don't think it's a solution for funding Open Source overall, in every possible edge case and for all the different ways that open source suffers from a lack of investment and funding. <br/><br/>
> There's this long tail of open source maintainers that are very individually motivated to create really interesting technology but they're not funded by anyone, they're just doing in their free time - evenings and weekends. Then there's this spike at the end of that tail where you've got maintainers motivated to continue building projects and growing their Open Source communities that are really huge. <br/><br/>
> Maybe these projects have gotten 10s of thousands of stars or millions of users and all of a sudden, the maintainer's like 'oh my gosh, not only am I building this thing and it's this cool community, but maybe I can start a company around it?'. <br/><br/>
> A lot of people are doing that, and that's the world that I focus on. I think GitHub can play in that world as well. They haven't yet. There's a lot of interesting things they can do there and I think GitHub can make it easier for people to get data and instrumentation about how the software is used.<br/><br/>
> There's a lot of fundamental realities with Open Source preventing anyone from from getting full visibility about the complete possible space of activity around Open Source adoption and usage and deployment and integration and embedding and all these other things. That's pretty pretty obvious to see why that is. I definitely think GitHub is going to innovate more.<br/><br/>
> The rise of the commercial Open Source founder as a role in the Open Source communities is really a thing. 10 years ago it was not a thing, there were probably less than a couple hundred, a few hundred commercial Open Source companies in the world of any size a decade ago, now there's thousands. <br/><br/>
> GitHub is a positive evolution, a positive force for amplifying our abilities as humans, and collaborating more efficiently and more productive with software creation. But it's also something that people should be really careful with just putting all their eggs in that one access control basket as it relates distributing your software, but also engaging with lots of stakeholders. <br/><br/>
> If you concentrate everything on GitHub I think it's a recipe for suboptimal business outcomes as a commercial Open Source founder and, over time, you should really be more in control over how you engage your Community, how you measure and control a lot of different aspects of engagement and interaction with your Community and with your end users, more importantly, not just your community.

**For those future Commercial Open Source project founders starting out today, who are thinking about building a company around their project, what options do they have today, or might have in the future?**

> There's some really interesting innovations. My friend Martine Casado funded a company called Orbit, which is like a smart CRM for community engagement. And there's a bunch of really interesting innovations here, lots of cool startups. <br/><br/>
> I haven't seen anything that solves this kind of problem. Other than a shift [to founders thinking] 'I've got a really awesome Open Source technology, everything lives on Github, but maybe I need to start to design and build different systems of engagement and systems of record for the way I track and measure and interact with my pen source community'. <br/><br/>
> I think we're just going to continue to see a lot of innovation there for sure.

Yeah I recognize all of those things that you were saying there, we've been through exactly the same journey, starting off as a small project that was scratching an itch for the founder to solve his day-to-day problems, to discovering that he was providing value to large enterprise organizations, to the next step on that journey to, as you say, extract that value without damaging the Community that you've already built up and the damaging the trust that you've already obtained.

**It's been great talking to you JJ, hopefully we can follow up again soon. I appreciate all of your advice and the benefit of your experience, thank you**.

> JJ: My pleasure, thanks for reaching out, Jonny. 
