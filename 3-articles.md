---
layout: page
title: Articles
permalink: /articles/
---

<h2>Articles</h2>
### Calls, code and comms.
<p>A series of posts about what makes research, design and development teams successful at creating new products.</p>

<ul>

{% for post in site.categories.article reversed  %}
    <li>
        <p><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></p>
        <p>{{ post.excerpt }}</p>
    </li>
{% endfor %}
</ul>
<br/>

<h2>Talks</h2>
<ul>
    <li>
        <p><a href="https://speakerdeck.com/jonny_robots/introduction-to-the-design-studio-methodology" target="_blank">Introduction to Design Studio <i class="fas fa-external-link-alt icon"></i></a> (2016) </p>
        <p>A workshop given to UX professionals on using "<a href="https://methods.18f.gov/discover/design-studio/" target="_blank">Design Studio</a>" methodology to engage and align your team and project stakeholders.</p>
    </li>
    <li>
        <p><a href="https://speakerdeck.com/jonny_robots/beyond-usability" target="_blank">Beyond Usability <i class="fas fa-external-link-alt icon"></i></a> (2016)</p>
        <p>A part-talk, part-workshop on developing a <a href="https://www.invisionapp.com/inside-design/guide-to-design-systems/" target="_blank">Design System</a> in order to progress the capability of your design team.</p>
    </li>
    <li>
        <p><a href="https://speakerdeck.com/jonny_robots/you-dont-need-a-ux-designer" target="_blank">You don't need a UX Designer <i class="fas fa-external-link-alt icon"></i></a> (2015)</p>
        <p>A talk given to an audience of UX professionals about the experience of teaching non-UX professionals to develop UX skills</p>
    </li>
</ul>

