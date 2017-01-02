---
layout: page
category: news
title: News
exclude: false
---

<ul class="post-list">
 	{% for post in site.posts %}
  	{% if post.categories contains 'news' %}
	 <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
        <p>{{ post.description }}</p>
      </li>
  {% endif %}
  {% endfor %}
</ul>