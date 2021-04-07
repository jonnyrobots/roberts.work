---
layout: post
title:  "Forming and operating a commercial OSS business"
abstract: More research into the commercial models behind commercial Open Source software companies, and an explanation of how OSS projects turn into revenue-generating companies.
permalink: /articles/forming-and-operating-coss/
date:   2021-03-03 21:03:00 +0000
readtime: 15 minutes
categories: article
---

# Forming & operating an OSS business 
### How Free OSS turns into Commercial OSS

In 2019 we acquired a company with an “open core” product. The simplest version of the product was provided for free, and available as Open Source software (OSS). On top of the free OSS (“FOSS”) version was a commercial version (“COSS”) that provided additional features targeted at a subset of user base.

That business was different in every way to the one that acquired it. It differed in commercial model (subscription vs. transactional), pricing model (per unit vs. per user), distribution model (OSS vs. proprietary), user interface (CLI vs. GUI), market, end user... there was a lot to understand. 

I’ve spent the last two years learning how to design, develop and manage the commercial success of that [product](https://www/flywaydb.org). This article is the result of my experience to date. It's also a reflection of the insights I've gained from conversations with investors, CPOs, CEOs, developers and other Product Managers who also built and operated OSS products and companies.

I’ve written this for Open Source project creators and maintainers. It's for people who have one eye on founding a company of their own. I hope it provides some useful guidance for how to think about creating and operating a COSS company.

**In this article**:
- [Forming & operating an OSS business](#forming--operating-an-oss-business)
    - [How Free OSS turns into Commercial OSS](#how-free-oss-turns-into-commercial-oss)
    - [What constitutes an “Open Source” business has changed​](#what-constitutes-an-open-source-business-has-changed)
    - [A COSS company is made in 3 movements](#a-coss-company-is-made-in-3-movements)
    - [Open Source means great distribution and ease of adoption](#open-source-means-great-distribution-and-ease-of-adoption)
    - [Capturing value is hard; SaaS is the modal mechanism](#capturing-value-is-hard-saas-is-the-modal-mechanism)
    - [Without observational reach, OSS users are stuck at 0](#without-observational-reach-oss-users-are-stuck-at-0)
    - [Developers engage in communities where they can learn](#developers-engage-in-communities-where-they-can-learn)
    - [Organisational structure and focus](#organisational-structure-and-focus)
      - [At movement 1 - Distribution and Adoption, Observability and Reach](#at-movement-1---distribution-and-adoption-observability-and-reach)
      - [At movement 2 - Awareness of paid-for, and Willingness to Pay](#at-movement-2---awareness-of-paid-for-and-willingness-to-pay)
      - [Movement 3 - Upsell to Enterprise](#movement-3---upsell-to-enterprise)
    - [Today’s $10-20k deal is tomorrow’s $500-$1m customer](#todays-10-20k-deal-is-tomorrows-500-1m-customer)

- - - 

<br/>

### What constitutes an “Open Source” business has changed​

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

### A COSS company is made in 3 movements

One of the great things about OSS projects are that they often start life as a solution to a problem the project founder experienced. Problems experienced in commercial settings (ie. experienced while being paid) have the most potential for being commercialised [^1]. How you get there happens in three movements.

| Movement | Name | Description | Success measure |
| - | - | - | - |
| 1 | Project-community fit | Have you solved a problem the community recognise? | Projects for developer community; **GitHub stars**. Requires “critical community mass” |
| 2 | Product-market fit | Is the solution being used? | For users, success measured in **downloads**. Requires organic adoption |
| 3 | Value-market fit | Do the employers of your users see value in paying for your product? | For buyers; success measured in **revenue**. Requires revenue from value to Enterprise |

One failure mode for commercialising OSS (or likely any new product, for that matter) is attempting to skip a movement. If your end goal is to commercialise your OSS project, then of course you need signals that you’re solving a valuable problem – one being that you were once paid to solve the problem - but you probably shouldn’t start by building a hosted service. 

This means being patient and disciplined. And this is important because commercial OSS companies typically have horrible free-to-paid conversion rates. Expect to convert just 1%-to-2% of your user base into customers. 

To succeed as a COSS business, you need a large Total Addressable Market (TAM) and a huge user base to convert. This is where Open Source comes in to its own: distribution. 

### Open Source means great distribution and ease of adoption 

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

### Capturing value is hard; SaaS is the modal mechanism 

When an Open Source project experiences success (see Fig. 2), it's time to "extract the value" created. This involves creating a commercial entity, coming up with something to sell and then marketing it.

There's no consensus for the "right" way to brand your commercial entity. Some people choose to name the company after the project (eg. Docker and Docker, Inc), others are happy for the two to be distinct (eg. Wordpress and Automaticc, Inc). Regardless, it is very important to own the trademark to the name of the OSS project, since this is the name users most readily associate with the software[^2].

Revenue for COSS businesses comes from the employers of the people using the OSS project. Beyond charging for "support" (see Fig. 1), company founders need to think past individual user needs, understand the commercial setting in which they're working and look to build what's valuable to the individual's team or organisation as a whole. 

Most COSS businesses opt for a Cloud-hosted product provided as SaaS. The value is usually captured by removing operational cost and adding in collaboration capabilities (which teams value) and compliance features (which Enterprise organisations value). 

None of this is any good if you don't have a relationship with your OSS user base. 

### Without observational reach, OSS users are stuck at 0

The biggest challenge to building a COSS business is how to market to the OSS user base. When you offload distribution of your OSS to GitHub, for example, you surrender control and with it useful information about who's consuming your code, how and where. Having “observational reach” is a key part of later being able to convert users into customers.

The "1-2-3" model illustrates this in the context of how an OSS project feeds into a COSS business. This table shows that progression from left to right.

| Stage | 0 | 1 | 2 | 3 |
| - | - | - | - | - |  
| **Type** | 👤 Individual | 👩‍💻 Individual | 👩‍💼👩‍💻👨‍💻 Team | 🏢 Enterprise | 
| **Status** | Unknown user | Community member (known) | Customer | Enterprise customer | 
| **Size** |100,000|50,000|2,000|100|
| **Value** | Creation  | Creation / Education | Collaboration | Compliance | 
| **Motion** | Free <br/>(OSS) | Free <br/>(Community) | Paid <br/>(Self serve) | Paid <br/>(Account sale) |
| **Metric** | Repo Stars | MAU | MRR | ACV |  

*Fig. 4. Table showing the "1-2-3" model[^3], with 0 added to account for state of no observational reach.*

Before it can successfully market a commercial offering, a COSS business needs to get observational reach into the user base to understand:

1. **Who the user base is**. It is hard to market to the OSS user base if they are anonymous (or even pseudonymous, as most GitHub accounts are). 
2. **How the software is used**. Most OSS projects with the potential to generate revenue solve problems at the infrastructure layer. Infrastructure is sensitive, which constrains options for telemetry.

Obtaining this understanding is fraught with technical (ie. how) and religious (ie. being a good OSS citizen) questions. But, failure to build user base visibility means failure full stop. NPM, which ended up being sold to GitHub is a good example of this. 

While Cloud-hosted SaaS is the logical product conclusion (today), it is a large, long-term investment. There are smaller investments that can and should be made along the way to increase engagement and permission to market to the user base.

Which brings us to Community.

### Developers engage in communities where they can learn

Commercial OSS companies generate less revenue per unit than closed-core (or “proprietary”) software businesses. Put simply, conversion rates for OSS are low. Very low. A typical COSS business should only expect to convert between 1 and 2 percent of its free OSS user base.

Subsequently, operating a successful (ie. profit-generating) COSS business requires an extremely large FOSS user base. Having a vibrant community is a key part of achieving this. 

Some things to remember when building a community:

- Where the community exists – LinkedIn, Slack, Discord – doesn’t matter in the first instance, but in time aspire to have control of the channel and the member list
- The "Community member" persona is much more likely to be a consumer of the software, as opposed to a contributor of code (although code isn't the only contribution an individual can make to an OSS project)
- The purpose of the Community should be to support the learning and development of members, which is accelerated by producing content 
- The subject of the content depends on where the product is in its lifecycle; OSS that's novel new technology might first focus on the behind-the-scenes detail to grow interest and early adopters 
- Documentation is the number 1 thing to get right. Aspire to answer every question about how to use the software directly, and then follow up by making sure that's captured in documentation

In time, the Community will become your main mechanism for observational reach and, done properly, earn you the right to increase awareness of the value in paying for the commercial version. But, it's important to recognise that there's a stage in between user base growth and conversion; awareness of paid value. 

One way to subtly increase awareness of paid value whilst still focusing on the core principle of Community value – education – is by producing a course. Spending time to create structured learning not only provides education for the participant but can also:

- Raise awareness of your product when course attendees share news of their accreditation with their network 
- Turn into a revenue stream itself if the course ends up being valuable enough to charge for
- Raise awareness of your paid-features by teaching concepts that rely on using paid features 

### Organisational structure and focus

As we saw earlier, *"a commercial OSS product/company is made in three movements"*, and each movement (also called "go-to-market" motion) has a corresponding focus. You need to be aware of all the motions, but you'll burn cash and attention trying to work on all of them at once. Unless your runway is wide and long, each motion is best tackled **one at a time, in order**, and applying the appropriate **organisational structure** at each. 

#### At movement 1 - Distribution and Adoption, Observability and Reach

In this motion it's usually just the project founder/maintainer and maybe some contributors (ensure a CLA is signed) working together. You're not organising yourself any differently to how you organise around writing code, but you should be beginning to broaden your activities.

At this point you are, at most, a small team of developers investing time in writing code and – critically – marketing the OSS project. It's got to be easy for others to discover and use it. 

Talk and write about the problem, it's always more interesting than the product. If the audience shares the problem, they want your opinions on solutions and they'll always find their way back to your product. 

The second part is Observability and Reach. Most people skip this because it's tricky, but knowing who's using your code and being able to engage with them is critical later. Best start now. 

Open Source licensing, expectations around telemetry and GitHub make work to separate you from users of your project and how they use your code. At this point you need to find ways to interact with your users to learn from them. For now, this can be as simple as a newsletter, but just make sure you can communicate with your users when you need to, ready for Movement 2. 

#### At movement 2 - Awareness of paid-for, and Willingness to Pay

In movement 2, you're still a core product/engineering team but you're beginning to exercise individual specialisms. Start with marketing and if all goes well, it'll be closely followed by sales. 

At this point, marketing is about raising the level of awareness within your community/free user base that a) there's a commercial product available, and b) there's absolute clarity in its value. 

You're an engineering team building the paid-for features, talking about them – in general terms and in sales calls, – and implementing the payment systems to charge for them.

#### Movement 3 - Upsell to Enterprise

At this point you've repeated the value discovery work and (probably) found yourself building a new Cloud SaaS product with compliance features for a new buyer persona. Now you're selling value to the employers of your users.

In the third movement you're organised in a way that's almost completely unrecognisable from 1 and 2. Product, Sales and Marketing are all separate specialised functions whose leadership teams still interact, but the day to day development, selling and promotional work happens efficiently and under the guidance of complementary strategies, objectives and success criteria. 

| | Motion 1 | | Motion 2 | | Motion 3 |
| - | - | - | - | - | - |  
| **Focus** | Distribution and adoption, and reach and observability | → | Raising awareness of commercial offering and willingness to pay | → | Capturing full value from Enterprise needs |
| **Roles** | Project founder (and contributors) | → | plus paid Software Engineers and DevEx | → | plus dedicated Product, Engineering, Sales and Marketing functions (and Legal) |
| **Activities** | Developing OSS features, interacting with Community peers and iterating on feedback, advocating solution | → | plus developing proprietary features/services, educating Community, providing support, marketing features, and selling | → | plus pricing and packaging, developing Enterprise features and meeting implementation needs (legal/compliance) |

*Fig. 5 – A summary of each of the three go-to-market motions*

### Today’s $10-20k deal is tomorrow’s $500-$1m customer

In the early days you'll celebrate every new customer you acquire, regardless of the additional ARR each brings. Then one day you'll bring in a big deal and those <$5k deals will start to look less interesting. 

One thing to note is that moving from movement 2 to 3 often leaves the lower value transactions without human interaction. A benefit of putting a human in charge of transactional sales is that it's a way to ensure the the gap to enterprise sales is bridged when those customers are ready. 

Elastic industrialised this with a group called “At Scale” - progressing the higher end of the long tail. Of course you should also align sales incentives to the things you want to sell.

It pays to be disciplined and continue to focus on landing those <$5k deals, because a healthy SaaS business is built on three metrics: ARR/MRR, MAU and NDR. 

- **ARR/MRR** - Annual Recurring Revenue / Monthly Recurring Revenue – how much recurring revenue do you have on an annual and monthly basis. 
- **MAU** – Monthly Active Users – how many people are actively using your product each month.
- **NDR** – Net Dollar Retention – take a group of customers from last year, and work out how much they're spending this year, compared to last. Positive percentages are a strong sign of a healthy COSS business. 

These three metrics (there are more) tell you how healthy your product business. Particularly NDR, because it shows you how "sticky" your product is (ie. how much your customers depends on it) and, importantly, whether those customers are coming back for more and increasing their spend with you each year and turning that first $5k deal into $10, then $20k, $100k and so on. 

<hr/>

**Footnotes**

[^1]: As an aside, this is one of the biggest potential disruptors to the UX industry as it dispatches the notion that “you are not your user”. 

[^2]: Owning the trademark doesn't mitigate this risk entirely – see Mongo and AWS – but it makes the risk manageable.  

[^3]: For more information on the 1-2-3 model see Adam Gross, former Heroku CEO, talk about [building self-serve go to market](https://www.heavybit.com/library/video/self-serve-go-to-market/).  