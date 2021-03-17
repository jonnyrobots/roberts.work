---
layout: post
title:  "Forming and operating a Commercial Open Source software company"
abstract: A explnation of how open source software projects turn into revenue-generating companies.
permalink: /articles/forming-operating-coss/
date:   2021-03-03 21:03:00 +0000
readtime: 7 minutes
---

# Forming and operating an Open Source software company

### How Open Source software projects turn into revenue-generating companies.

In 2019 we acquired a company with an “open core” product. The simplest version of the product was provided for free, available as Open Source software (OSS). On top of the free OSS (“FOSS”) version was a commercial version (“COSS”) with additional features targeted at a subset of the total user base.

That business was different in every way to the one that acquired it: in commercial model (subscription), pricing model (per unit), distribution model (OSS), user interface (CLI), market, end user... there was a lot to understand. 

I’ve spent the last two years learning how to design, develop and operate that product and the business around it. This article is the result of my research conversations with investors, CPOs, CEOs and developers who built companies out of their open source projects.

I hope it's useful to Open Source project founders interested in founding companies.  

**In this article**:

1. [What constitutes an Open Source business has changed over time]()
2. [A commercial OSS product/company is made in three movements]()
3. [Open Source means great distribution and ease of adoption]()
4. [Capturing value from OSS is hard; Cloud SaaS is the most prevalent solution]()
5. ⏳ [The todo list is infinite; what needs doing next depends on where your product is in its life]() 
6. ⏳ [Without observational reach, OSS users are stuck at 0 in the 1-2-3 model]()
7. ⏳ [Developers engage in communities where they can learn]()
8. ⏳ [The org structure for delivering at “1” & “2” is necessarily different to “3”]()
9. ⏳ [Today’s $10-20k deal is tomorrow’s $500-$1m customer]()



<br/>
- - - 

<br/>

### What constitutes an “Open Source” business has changed over time​

There is no standard definition for “open source”. How you choose to define it depends largely on the OSS project you’re talking about, and the period of time in which you’re talking.

This table is an illustration of my understanding of how the Venture Capital (VC) firm Andreessen-Horrowitz (aka “A16Z”) chooses to define it.   

| Period | Phase | OSS Seen as |
| --- | --- | --- |
| ‘70’s - ‘90’s | Open Source 0.0 | “free software” |
| ‘90’s - ‘00’s | Open Source 1.0 | “support and services” |
| ‘00’s - ‘20’s | Open Source 2.0 | “SaaS on top” |
| ‘20’s - ‘30’s | Open Source 3.0 | ‘Big Tech’ “exhaust” |

The last row in the table is speculation based on the growing trend of OSS projects originating as a by-product of ‘Big Tech’ as it works on its core business. Unless you’re a VC, or run a successful software business at scale, ignore this.

Also beware of the “Period” column. You may be tempted to infer, for example, that a COSS company offering support and services is a bit “nineties”. Instead, this column should be read as “your only option for commercialisation in the ’90’s was through support and services”. 

Today, most COSS companies are most recognisable as “Open Source 2.0”. These OSS projects are created and commercialised through “as a Service” offerings. MongoDB (OSS) and Mongo Atlas (SaaS) are a perfect example of this. However, “Phase” is important, and for OSS project founders, it’s useful to think about each as an incremental step as you grow your product and company. As we’re about to see.

### A commercial OSS product/company is made in three movements

One of the great things about OSS projects are that they often start life as a solution to a problem the project founder experienced. Problems experienced in commercial settings (ie. experienced while being paid) have the most potential for being commercialised [^ As an aside, this is one of the biggest potential disruptors to the UX industry as it dispatches the notion that “you are not your user”.]. How you get there happens in three movements.

| Movement | Name | Description | Success measure |
| - | - | - | - |
| 1 | Project-community fit | Have you solved a problem the community recognise? | Projects for developer community; **GitHub stars**. Requires “critical community mass” |
| 2 | Product-market fit | Is the solution being used? | For users, success measured in **downloads**. Requires organic adoption |
| 3 | Value-market fit | Do the employers of your users see value in paying for your product? | For buyers; success measured in **revenue**. Requires revenue from value to Enterprise |

One failure mode for commercialising OSS (or likely any new product, for that matter) is attempting to skip a movement. If your end goal is to commercialise your OSS project, then of course you need signals that you’re solving a valuable problem – one being that you were once paid to solve the problem - but you probably shouldn’t start by building a hosted service. 

This means being patient and disciplined. And this is important because commercial OSS companies typically have horrible free-to-paid conversion rates. Expect to convert just 1%-to-2% of your user base into customers. 

To succeed as a COSS business, you need a large Total Addressable Market (TAM) and a huge user base to convert. This is where Open Source comes in to its own: distribution. 

### "Open Source" means great distribution and ease of adoption 

The most compelling reason to build a company on top of an OSS project is distribution. Or put another way, the reason most COSS companies are born into existence is because of the _incredible distribution OSS affords_.

When you decide to create a product, one of your most pressing concerns will be how to get that product into the hands of users and customers. For software companies who sell software to other companies ("B2B"), this equates to time (and money) spent convincing people in those companies to try your product.

By choosing to take the Open Source route, you offload a huge amount of the complexity in distribution and are rewarded with a simple way to get something of value into the hands of your end users. 

Here's an overview of concerns mitigated by OSS:

| Persona | Concern | OSS mitigation | 
| - | - | - |
| End user | Budget | OSS is (generally) free |
| End user | Availability | GitHub etc |
| End user | Time spent learning | Self-supporting communities | 
| IT Admin | IT/security approval | Code easily scanned | 
| Legal | Licensing conditions | Permissive licensing (eg. Apache) |

When looking at Open Source as a distribution mechanism our focus is on consumption, and not contribution. This is an important differentiation to make. The vast majority of people who interact with OSS projects do so as users – consumers of the software – and not as contributors (ie. developers) of it.

Creators of OSS projects, with aspirations to found companies should look at OSS as a mechanism that enables fantastic "top of funnel" growth. 

So, where's the downside...?

### Capturing value from OSS is hard; Cloud SaaS is the most prevalent mechanism 

Capturing value from OSS is hard; Cloud SaaS the most prevalent mechanism

When an Open Source project experiences success (see Fig. 2), it's time to "extract the value" created. This involves creating a commercial entity, coming up with something to sell and then marketing it.

There's no consensus for the "right" way to brand your commercial entity. Some people choose to name the company after the project (eg. Docker and Docker, Inc), others are happy for the two to be distinct (eg. Wordpress and Automaticc, Inc). Regardless, it is very important to own the trademark to the name of the OSS project, since this is the name users most readily associate with the software[^ Owning the trademark doesn't mitigate this risk entirely – see Mongo and AWS – but it makes the risk manageable].

As for *what* to sell, that's laid out in Fig. 1. Depending on the complexity of your code, the most obvious first paid-for feature is "support"; allowing customers to tap you up for your knowledge of the software and the problem space.

Revenue for COSS businesses comes from the employers of the people using the OSS project. Beyond "support", company founders need to think past individual user needs and understand the commercial setting in which they're working. 

The biggest challenge to building a COSS business is how to market. When you offload distribution of your OSS toGitHub, let's say, you surrender control and with it useful information about who's consuming your code, how and where. You lack “observational reach”, and getting it is hard work that involves trying to talk to your users. 

This is where having a healthy OSS project community comes in useful.

Most COSS businesses though opt for a Cloud-hosted product provided as SaaS where the value is in removing the operational cost and adding in collaboration features (which teams value) and compliance features (which Enterprise organisations value). A free tier provides a way to achieve observational reach via the service, and to market to them as a quid pro quo for free use of the (usually limited) service. 

| Level | 0 | 1 | 2 | 3 |
| - | - | - | - | - |  
| **Type** | 👤 <br/>Individual | 👩‍💻 <br/>Individual | 👩‍💼👩‍💻👨‍💻 <br/>Team | 🏢 <br/>Enterprise | 
| **Status** | Unknown | Community member | Customer | Enterprise customer | 
| **Value** | Creation  | Creation / Education | Collaboration | Compliance | 
| **GTM** | OSS (free) | Community (free) | Paid (self serve) | Paid (Account sale) |
| **Metrics** | None | MAU | MRR | ACV |  

*Fig. 4. Table showing the "1-2-3" model[^Cf. Adam Gross], with 0 added to account for state of no observational reach.*
