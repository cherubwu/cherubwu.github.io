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
  <br><hr>
  <div class="post">
    <h3 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h3>
    <span class="post-date">{{ post.date | date_to_string }}</span>
    {{ post.excerpt }}
  </div>
  {% endfor %}
</div>
