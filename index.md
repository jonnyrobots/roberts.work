---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Writing
exclude: true
---

<ul class="article-list">
{% for post in site.posts limit:25 %}
{% unless post.unlisted %}
<li>
<span class="postname"><a href="{{ site.baseurl }}{{ post.url }}" >{{ post.title }}</a></span><span class="timestamp">{{ post.date | date: "%d %b %y" }}</span>
</li>
{% endunless %}
{% endfor %}
</ul>



