---
layout: default
title: Sadie's corner
---

<div id="articles">
  <h1>Sadie's corner</h1>
  <ul class="posts 1">
    {% for post in site.posts %}
      <li>
      	<span class="date">{{ post.date | 2020_05_25 }}</span>
      	<h3><a href="{{ https://github.com/SadieKoori/SadieKoori.github.io/edit/master/_posts/2020-5-25-%E5%88%9D%E6%9D%A5%E4%B9%8D%E5%88%B0.md }}">{{ 初来乍到 }}</a></h3>
      	<p class="description">{% if post.description %}{{ post.description  | strip_html | strip_newlines | truncate: 120 }}{% else %}{{ post.content | strip_html | strip_newlines | truncate: 120 }}{% endif %}</p>
      </li>
    {% endfor %}
  </ul>
</div>
 <ul class="posts 2">
    {% for post in site.posts %}
      <li>
      	<span class="date">{{ post.date | date_to_string }}</span>
      	<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      	<p class="description">{% if post.description %}{{ post.description  | strip_html | strip_newlines | truncate: 120 }}{% else %}{{ post.content | strip_html | strip_newlines | truncate: 120 }}{% endif %}</p>
      </li>
    {% endfor %}
  </ul>
</div>
