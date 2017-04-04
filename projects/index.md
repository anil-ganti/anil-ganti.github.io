---
layout: page
title: Projects
excerpt: "An archive of articles sorted by date."
search_omit: true
image:
  feature: projects_splash.jpg
---

<ul class="post-list">
{% for post in site.categories.projects %} 
  <li><article>{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.author | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %} {{ post.excerpt }}</article></li>
{% endfor %}
</ul>
