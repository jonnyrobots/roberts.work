---
layout: page
title: Projects
permalink: /projects/
---

<h1>Projects</h1>

<ul>
{% for post in site.categories.project  %}
    <li>
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
        <p>{{ post.excerpt }}</p>
        <span class="project-category">{{ post.tags }}</span>
    </li>
{% endfor %}
</ul>

