---
layout: page
title: Designance
permalink: /designance/
---

# Designance
<iframe height="320" src="https://designance.substack.com/embed" frameborder="0" scrolling="no" allowfullscreen></iframe>

<p>Designance is a newsletter I write while exploring the principles of design and finance, pitting my investing skills against creating a product of my own.</p>

<p>Subscribe to get the latest instalment delivered straight to your inbox, or read the archive below. And if you like what you're reading, consider forwarding it to a friend.</p>

### Archive

<ul class="newsletter">
{% for post in site.categories.designance %}
    <li>
        <a href="{{ site.baseurl }}{{ post.url }}" title="Read {{ post.title }}">
            <span>
                {{ post.image }}
                <p class="datestamp">{{ post.date | date_to_long_string }}</p>
                <h3>{{ post.title }}</h3>
                <p>{{ post.subtitle }}</p>
            </span>
        </a>
    </li>
{% endfor %}
</ul>



