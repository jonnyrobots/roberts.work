---
layout: post
title:  "Forming and operating a Commercial Open Source software company"
abstract: A explnation of how open source software projects turn into revenue-generating companies.
permalink: /articles/forming-and-operating-coss/
date:   2021-03-03 21:03:00 +0000
readtime: 10 minutes
---

# Forming and operating an Open Source software company

In 2019 we acquired a company with an “open core” product. The simplest version of the product was provided for free, available as Open Source software (OSS). On top of the free OSS (“FOSS”) version was a commercial version (“COSS”) with additional features targeted at a subset of the total user base.

That business was different in every way to the one that acquired it: in commercial model (subscription), pricing model (per unit), distribution model (OSS), user interface (CLI), market, end user... there was a lot to understand. 

I’ve spent the last two years learning how to design, develop and operate that product and the business around it. This article is the result of my research conversations with investors, CPOs, CEOs and developers who built companies out of their open source projects.

I hope it's useful to Open Source project founders interested in founding companies.  

**In this article**:
- [Forming and operating an Open Source software company](#forming-and-operating-an-open-source-software-company)
  - [What constitutes an “Open Source” business has changed over time​](#what-constitutes-an-open-source-business-has-changed-over-time)
  - [A commercial OSS product/company is made in three movements](#a-commercial-oss-productcompany-is-made-in-three-movements)
  - ["Open Source" means great distribution and ease of adoption](#open-source-means-great-distribution-and-ease-of-adoption)
  - [Capturing value from OSS is hard; Cloud SaaS is the most prevalent mechanism](#capturing-value-from-oss-is-hard-cloud-saas-is-the-most-prevalent-mechanism)
  - [Without observational reach, OSS users are stuck at 0](#without-observational-reach-oss-users-are-stuck-at-0)
  - [Developers engage in communities where they can learn](#developers-engage-in-communities-where-they-can-learn)
  - [⏳ Organisational structure and focus](#-organisational-structure-and-focus)
  - [⏳ Today’s $10-20k deal is tomorrow’s $500-$1m customer](#-todays-10-20k-deal-is-tomorrows-500-1m-customer)

- - - 

<br/>

## What constitutes an “Open Source” business has changed over time​

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

## A commercial OSS product/company is made in three movements

One of the great things about OSS projects are that they often start life as a solution to a problem the project founder experienced. Problems experienced in commercial settings (ie. experienced while being paid) have the most potential for being commercialised [^1]. How you get there happens in three movements.

| Movement | Name | Description | Success measure |
| - | - | - | - |
| 1 | Project-community fit | Have you solved a problem the community recognise? | Projects for developer community; **GitHub stars**. Requires “critical community mass” |
| 2 | Product-market fit | Is the solution being used? | For users, success measured in **downloads**. Requires organic adoption |
| 3 | Value-market fit | Do the employers of your users see value in paying for your product? | For buyers; success measured in **revenue**. Requires revenue from value to Enterprise |

One failure mode for commercialising OSS (or likely any new product, for that matter) is attempting to skip a movement. If your end goal is to commercialise your OSS project, then of course you need signals that you’re solving a valuable problem – one being that you were once paid to solve the problem - but you probably shouldn’t start by building a hosted service. 

This means being patient and disciplined. And this is important because commercial OSS companies typically have horrible free-to-paid conversion rates. Expect to convert just 1%-to-2% of your user base into customers. 

To succeed as a COSS business, you need a large Total Addressable Market (TAM) and a huge user base to convert. This is where Open Source comes in to its own: distribution. 

## "Open Source" means great distribution and ease of adoption 

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

## Capturing value from OSS is hard; Cloud SaaS is the most prevalent mechanism 

Capturing value from OSS is hard; Cloud SaaS is the most prevalent mechanism

When an Open Source project experiences success (see Fig. 2), it's time to "extract the value" created. This involves creating a commercial entity, coming up with something to sell and then marketing it.

There's no consensus for the "right" way to brand your commercial entity. Some people choose to name the company after the project (eg. Docker and Docker, Inc), others are happy for the two to be distinct (eg. Wordpress and Automaticc, Inc). Regardless, it is very important to own the trademark to the name of the OSS project, since this is the name users most readily associate with the software[^2].

Revenue for COSS businesses comes from the employers of the people using the OSS project. Beyond charging for "support" (see Fig. 1), company founders need to think past individual user needs, understand the commercial setting in which they're working and look to build what's valuable to the individual's team or organisation as a whole. 

Most COSS businesses opt for a Cloud-hosted product provided as SaaS. The value is usually captured by removing operational cost and adding in collaboration capabilities (which teams value) and compliance features (which Enterprise organisations value). 

None of this is any good if you don't have a relationship with your OSS user base. 

## Without observational reach, OSS users are stuck at 0

The biggest challenge to building a COSS business is how to market to the OSS user base. When you offload distribution of your OSS to GitHub, for example, you surrender control and with it useful information about who's consuming your code, how and where. Knowing this and having “observational reach” is key to converting users into customers.

The "1-2-3" model illustrates this in the context of how an OSS project feeds into a COSS business. This table shows that progression from left to right.

| Stage | 0 | 1 | 2 | 3 |
| - | - | - | - | - |  
| **Type** | 👤 Individual | 👩‍💻 Individual | 👩‍💼👩‍💻👨‍💻 Team | 🏢 Enterprise | 
| **Status** | Unknown user | Community member (known) | Customer | Enterprise customer | 
| **Size** |100,000|50,000|2,000|100|
| **Value** | Creation  | Creation / Education | Collaboration | Compliance | 
| **Motion** | Free <br/>(OSS) | Free <br/>(Community) | Paid <br/>(Self serve) | Paid <br/>(Account sale) |
| **Metric** | Repo Stars | MAU | MRR | ACV |  

*Fig. 4. Table showing the "1-2-3" model[^2], with 0 added to account for state of no observational reach.*

Before it can successfully market a commercial offering, a COSS business needs to get observational reach into the user base to understand:

1. **Who the user base is**. It is hard to market to the OSS user base if they are anonymous (or even pseudonymous, as most GitHub accounts are). 
2. **How the software is used**. Most OSS projects with the potential to generate revenue solve problems at the infrastructure layer. Infrastructure is sensitive, which constrains options for telemetry.

Obtaining this understanding is fraught with technical (ie. how) and religious (ie. being a good OSS citizen) questions. But, failure to build user base visibility means failure full stop. NPM, which ended up being sold to GitHub is a good example of this. 

While Cloud-hosted SaaS is the logical product conclusion (today), it is a large, long-term investment. There are smaller investments that can and should be made along the way to increase engagement and permission to market to the user base.

Which brings us to Community.

## Developers engage in communities where they can learn

Commercial OSS companies generate less revenue per unit than closed-core (or “proprietary”) software businesses. Put simply, conversion rates for OSS are low. Very low. A typical COSS business should only expect to convert between 1 and 2 percent of its free OSS user base.

Subsequently, operating a successful (ie. profit-generating) COSS business requires an extremely large FOSS user base. Having a vibrant community is a key part of achieving this. 

Some things to remember when building a community:

- Where the community exists – LinkedIn, Slack, Discord – doesn’t matter in the first instance, but in time aspire to have control of the channel and the member list
- The "Community member" persona is much more likely to be a consumer of the software, as opposed to a contributor of code (although code isn't the only contribution an individual can make to an OSS project)
- The purpose of the Community should be to support the learning and development of members, which is accelerated by producing content 
- The subject of the content depends on where the product is in its lifecycle; OSS that's novel new technology might first focus on the behind-the-scenes detail to grow interest and early adopters 
- Documentation is the number 1 thing to get right. Aspire to answer every question about how to use the software directly, and then follow up by making sure that's captured in documentation

In time, the Community will become your main mechanism for observational reach and, done properly, earn you the right to increase awareness of the value in paying for the commercial version. But, it's important to recognise that there's a stage in between user base growth and conversion; awareness of paid value. 

One way to subtly increase awareness of paid value whilst still focusing on the core principle of Community value – education – is by producing a  course. Spending time to create structured learning not only provides education for the participant but can also:

- Raise awareness of your product when course attendees share news of their accreditation with their network 
- Turn into a revenue stream itself if the course ends up being valuable enough to charge for
- Raise awareness of your paid-features by teaching concepts that rely on using paid features 

## ⏳ Organisational structure and focus

## ⏳ Today’s $10-20k deal is tomorrow’s $500-$1m customer

<hr/>

**Footnotes**

[^1]: As an aside, this is one of the biggest potential disruptors to the UX industry as it dispatches the notion that “you are not your user”.
[^2]: Owning the trademark doesn't mitigate this risk entirely – see Mongo and AWS – but it makes the risk manageable
[^3]: For more information on the 1-2-3 model see Adam Gross, former Heroku CEO, talk about [building self-serve go to market](https://www.heavybit.com/library/video/self-serve-go-to-market/).  