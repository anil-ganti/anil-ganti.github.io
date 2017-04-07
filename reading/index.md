---
layout: page
title: Reading List
excerpt: "An archive of articles sorted by date."
search_omit: true
image:
  feature: reading_splash.jpg
---

## Currently reading
<ul class="post-list">
{% for post in site.categories.reading %}
	<div class="container">
  <div class="overlay">
    <div class="text">{{ post.notes }}</div>
  </div>
  <img src="{{ site.url }}/images/{{ post.image.feature }}" width="100" height="120" style="float:left;">
  <li style="margin-left:120px">
  <article style="{font-size:24px}">{{ post.title }} 
  <span class="entry-date"></span>{% if post.excerpt %} <span class="excerpt" style="font-size:18px;">{{ post.author | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %} <i style="color:grey;font-size:20px">{{ post.excerpt }}</i></article></li>
  </div>
{% endfor %}
</ul>

## Recently read

<ul class="post-list">
{% for post in site.categories.read %}
  <div class="container">
  <div class="overlay">
    <div class="text">{{ post.notes }}</div>
  </div>
  <img src="{{ site.url }}/images/{{ post.image.feature }}" width="100" height="120" style="float:left;">
  <li style="margin-left:120px">
  <article style="{font-size:24px}">{{ post.title }} 
  <span class="entry-date"></span>{% if post.excerpt %} <span class="excerpt" style="font-size:18px;">{{ post.author | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %} <i style="color:grey;font-size:20px">{{ post.excerpt }}</i></article></li>
  </div>
{% endfor %}
</ul>