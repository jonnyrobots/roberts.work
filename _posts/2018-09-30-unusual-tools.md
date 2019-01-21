---
layout: post
title:  "Pt.2 - Writing: an unusual tool for research"
date:   2018-09-30 19:31:12 +0000
categories: article
---

How writing is fundamental to the product development process.

## Writing code: an unusual tool for research

![Drill]({{ site.baseurl }}/images/drill.png)

Out picking up a new drill this weekend, I remembered a quote we sometimes refer to as we carry out our research projects:

> “people do not want a quarter-inch drill, they want a quarter inch hole.”, Theodore Levitt

It’s one of the many nudges that we use in [Foundry](https://www.red-gate.com/foundry/#how-foundry-works) (Redgate’s Research and Development division) to keep learning until we’ve properly understood what our customers ultimate desired outcome is so we can design the right product.

Back at home, my tools usually end up strewn across the house — both specialist tools and common ones — and they get brought back to me to put away. Since scrap metal can be indiscernible from specialist tools, that gets brought back to me too. All this got me thinking about the selection of tools we use to carry out our research.

In the same way that it’s easy to confuse a piece of scrap metal with a specialist tool, it’s possible to misunderstand the valuable contribution to research that some less-obvious activities make.

It isn’t immediately obvious, for example, how important writing is to great research, but we’ve found it to be one of the most valuable research tools we have. In our research there are two types of writing; writing **blog posts** and writing **code**.

### Writing code

The majority of the Foundry team are software engineers. Being able to write code is a core competency. People interested in joining the team often ask how much time an engineer spends writing code compared to research. I understand the question, but it’s the wrong way to think about it. Research forms 100% of our work; code is just one of the activities we use to learn (around two thirds of the time we find it’s the right method to use).

We get research value from writing code in three ways; building **concept demos**, carrying out **technology exploration** and developing **prototype software**.

#### Concept demos

After collecting information and developing ideas, architects build architectural models. These scaled-down models are rarely built from the same materials as the final structure, but they allow the study of different aspects of the architectural design and can be used to communicate design ideas.

We emulate this with “**concept demos**”. Using HTML, CSS and JavaScript (usually React), we’re able to use them to explore some of the more complex scenarios (like identifying and classifying sensitive data) with our research participants.

#### Technology exploration

![Screwdriver]({{ site.baseurl }}/images/screwdriver.png)

In the same way an architect may choose to explore the use of new materials or building techniques, we also write code to carry out **technology explorations** in order to evaluate new ways of delivering software, or get become more efficient in our approach to research.

Exploring the use of [Electron](https://electronjs.org/) for two of our prototype products meant we could understand how to benefit from using web technologies whilst continuing to deliver software in a way that our customers are comfortable with.

Using natural language processing ([NLP](https://en.wikipedia.org/wiki/Natural_language_processing)) we’ve been able to analyse large amounts of unstructured data to uncover changes in the preference of technology stacks. With Machine Learning we’re able to push our prototypes further in terms of their “intelligence”, making important yet time-consuming tasks, such as sensitive data detection, more efficient.

#### Prototype software

Each of our research activities have one goal in common, and that’s to build our confidence in continuing to pursue a project (or cease working on it). The amount of investment we make, in terms of code, is directly equivalent to the amount of confidence we have in that solution.

At our most confident, we’re able to commit the time to developing **prototype software**. This is working software that evolves as we work closely with our most engaged users. In 2016 we built [Data Platform Studio](https://www.dataplatformstudio.com/) — DPS (an ingeniously simple import tool for Microsoft Azure) — and this year we built two working prototypes for regulatory compliance tasks; one to [audit and simplify database access](https://www.red-gate.com/blog/audit-and-compliance/sql-census-update-new-server-view), and the other to [mask sensitive data](https://www.red-gate.com/blog/audit-and-compliance/sql-data-mask) held within a database. Both are being developed as part of Redgate’s [Data Privacy and Protection](https://www.red-gate.com/blog/audit-and-compliance) offering.

### Writing blog posts

Writing code to learn really works for us once we’ve committed that learning to paper (or screen, really). Writing about what we’ve learned over the course of a research project has three benefits; it **consolidates learning**, provides the opportunity to **reflect back** and **builds confidence** in committing to a solution.

#### Consolidate learning

In Foundry we regularly check in with Redgate’s product portfolio managers. In these check-ins we’re asked difficult and reaching questions about what we’re learned and why the business should continue to invest in each project. Given the nature of the work we do, and the amount of ambiguity that surrounds our work it can be difficult to articulate what we’ve learned.

Taking the time to write a blog post gives us the space and time to synthesise that information. We’re able to **consolidate our learning** and present it as coherently as possible.

### Reflecting back

![Spirit level]({{ site.baseurl }}/images/level.png)

We write blog posts to achieve something similar to Reflective Listening; an interviewing method of confirming your understanding of what a participant is telling you. We invite our readers to comment on our posts. **Reflecting back** in this way confirms or corrects our understanding. More often than not it creates new opportunities for us to learn.

We also think it’s just good form to share back with the community that we’re learning from. Writing about the problem is more important than writing about your product. The most recent example of this is our series on Adopting Kubernetes step by step, a step by step guide outlining our experience and advice regarding a move to using Kubernetes.

#### Building confidence

In the early days of any project we’re searching for the signals that indicate it’s worth pursuing. We might we feel strongly that it is, but the signals may be weak.

Because writing prototype code can be expensive — we call it prototype code, but we believe strongly in quality and robust code — we need some strong signals. Writing a post about how the prototype will work, and then measuring the response to that post helps with **building confidence** in a solution before we’ve committed too much time to developing the wrong thing.

### The complete toolkit

![Toolkit]({{ site.baseurl }}/images/toolbox.png)

Indulge me as I hammer home the construction metaphor one last time. It’s important to pick the right tool for the job. We’ve found that writing code and blog posts make an enormous contribution to our objective of delivering new product opportunities to Redgate, but it’s important to create your own toolkit.

Before writing code or articles we have to talk with experts, interview a broad range of people and read about and understand new concepts before we begin to converge. Only then can we use writing as a research tool.

The best toolkits evolve over time as you learn which ones work best for each task. The more you use each of the tools, and increase your adoption of new ones, the more efficient your research will become.

<p style="text-align: center">. . .</p>
