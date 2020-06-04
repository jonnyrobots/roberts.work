---
layout: page
title: Articles
permalink: /articles/
---

<h2>Articles</h2>

### On research, design & development

<ul class="article-list">
{% for post in site.categories.article %}
<li>
<h4><a href="{{ site.baseurl }}{{ post.url }}" >{{ post.title }}</a></h4>
<p><strong>{{ post.date | date_to_long_string }}</strong> – ⏱ {{ post.readtime }}</p>
<p>{{ post.abstract }}<a href="{{ site.baseurl }}{{ post.url }}" title="Continue reading"> ...read → </a></p>
</li>
{% endfor %}
</ul>


<h2>Talks</h2>
### Recordings and slides of talks given
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