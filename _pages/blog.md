---
layout:     page
title:      Illustration 👩🏻‍🎨
permalink:  /illustration
nav_order:  3
---
 
![gh](/illustrations/gh.png){:class="img-responsive"}
<p style="text-align:center;color:gray;font-size:80%;">
La terre a une âme, elle est une créature vivante.<br>
&#128205; --Gustave Flaubert
</p>
 <h3><i class="fa fa-tag" aria-hidden="true"></i>&nbsp;{{ category[0] }}&nbsp;({{ category[1].size }})</h3>
  <ul style="list-style-type:none;">
    {% assign sorted_posts = category[1] | sort: 'title' %}
    {% for post in sorted_posts %}
      <li><i class="fa fa-file-text"></i>&nbsp;<a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}