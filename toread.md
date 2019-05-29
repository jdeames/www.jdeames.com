---
layout: kidpages
lang: en
title: excerpts
permalink: /excerpts/
exclude: false
published: true
---

<ul class="post-lineup">
 	{% for post in site.posts %}

	 <li>
        <h4><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h4>     
        <p>{{ post.description }}</p>
      </li>

  {% endfor %}
</ul>