---
layout:     page
title:      Blog
permalink:  /blog
nav_order:  3
---

![duty-calls](https://imgs.xkcd.com/comics/duty_calls.png){:class="img-responsive"}
<p style="text-align:center;color:gray;font-size:80%;">
Source: <a href="https://xkcd.com/386/">xkcd.com</a>.
</p>

{% assign sorted_categories = site.categories | sort %}
{% for category in sorted_categories reversed %}
  <h3><i class="fa fa-tag" aria-hidden="true"></i>&nbsp;{{ category[0] }}&nbsp;({{ category[1].size }})</h3>
  <ul style="list-style-type:none;">
    {% assign sorted_posts = category[1] | sort: 'title' %}
    {% for post in sorted_posts %}
      <li><i class="fa fa-file-text"></i>&nbsp;<a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}