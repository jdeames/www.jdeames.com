---
layout: page
category: excerpts
lang: en
title: excerpts
exclude: false
---

<ul class="post-lineup">
 	{% for post in site.posts %}

	 <li>
        <h4><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h4>     
        <p>{{ post.description }}</p>
      </li>

  {% endfor %}
</ul>