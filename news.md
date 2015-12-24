---
layout: post
permalink: /news/
title: News

---

<ul class="post-list">
{% for news in site.news reversed %}
    <li>
        <h3><a class="news-title" href="{{ news.url | prepend: site.baseurl }}">{{ news.title }}</a></h3>
        <p class="post-meta">{{ news.date | date: '%B %-d, %Y' }}</p>
        <p class="post-meta">{{news.description}}</p>
      </li>
{% endfor %}
</ul>