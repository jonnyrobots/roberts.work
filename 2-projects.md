---
layout: page
title: Projects
permalink: /projects/
exclude: true 
---

<h1>Projects</h1>

<ul>
{% for post in site.categories.project  %}
    <li>
        <p><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></p>
        <span class="postdate">{{ post.date | date_to_long_string }}</span>
        <p>{{ post.excerpt }}</p>
        <span class="project-category">{{ post.tags }}</span>
        
    </li>
{% endfor %}
</ul>

