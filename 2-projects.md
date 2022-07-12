---
layout: page
title: Projects
permalink: /projects/ 
---

Insight for people working on early- and growth-stage products 

<iframe src="https://embeds.beehiiv.com/713db3ef-4447-4b6f-8670-a9fcf96f33dd?slim=true" data-test-id="beehiiv-embed" frameborder="0" scrolling="no" style="margin: 0; border-radius: 0px !important; background-color: transparent;"></iframe>

### Projects

<ul class="article-list">
{% for post in site.categories.project %}
{% unless post.exclude %}
<li>
<span class="postname"><a href="{{ site.baseurl }}{{ post.url }}" >{{ post.title }}</a></span><span class="timestamp">{{ post.date | date: "%d %b %y" }}</span>
</li>
{% endunless %}
{% endfor %}
</ul>







