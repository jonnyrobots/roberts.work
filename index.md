---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
exclude: true 
title: Commercial strategy, research and design
---

<iframe src="https://embeds.beehiiv.com/713db3ef-4447-4b6f-8670-a9fcf96f33dd?slim=true" data-test-id="beehiiv-embed" frameborder="0" scrolling="no" style="margin: 0; border-radius: 0px !important; background-color: transparent;"></iframe>



<ul class="article-list">
{% for post in site.categories.article %}
<li>
<a href="{{ site.baseurl }}{{ post.url }}" >{{ post.title }}</a> <span>{{ post.date | date: "%d %b %y" }}</span>
</li>
{% endfor %}
</ul>



