---
layout: page
title: Recent reading list
excerpt: "An archive of articles sorted by date."
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.articles %}
  <li><article>{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.author | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %} <i>{{ post.excerpt }}</i></article></li>
{% endfor %}
</ul>
