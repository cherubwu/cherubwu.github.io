---
layout:     page
title:      Home
permalink:  /home
nav_order:  1
pagination: 
  enabled: true
---
<div class="posts">
  {% for post in site.posts %}
  <hr>
  <div class="post">
    <h3 class="post-title">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h3>
    <span class="post-date">{{ post.date | date_to_string }}</span>
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    <a class="read-more" href="{{ post.url }}">Read more &rarr;</a>
  </div>
  {% endfor %}
</div>

<style>
.post-excerpt { color: #666; margin: 0.5rem 0 0.3rem; line-height: 1.6; }
.read-more { font-size: 0.8rem; letter-spacing: 0.05em; color: #aa759f; text-decoration: none; }
.read-more:hover { text-decoration: underline; }
</style>
