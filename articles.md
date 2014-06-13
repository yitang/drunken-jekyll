---
layout: default
title: Articles
permalink: /articles/
---

<h1 class="dj-index-title">Recent Articles</h1>

<ul class="dj-index-post-list">
{% for post in site.posts limit:10 %} 
  <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="dj-index-entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></li>
{% endfor %}
</ul>