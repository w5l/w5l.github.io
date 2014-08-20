---
title: Home
layout: default
order: -1
permalink: /
---

I am gone to play outside untill further notice.

<ul class='postlist'>
  {% for post in site.posts limit:4 %}
  <li>
    <h3><a href='{{ post.url | prepend: post.baseurl }}'>{{ post.title }}</a> <small>&bull; {{ post.date | date: "%Y-%m-%d"}}</small></h3>
        <a href='{{ post.url | prepend: post.baseurl }}' class='inconspicuous'>
      {{ post.excerpt | remove: '<p>' | remove: '</p>' }}
    </a>
  </li>
  {% endfor %}
</ul>

* [Moto-Guzzi Superalce drivers manual](/superalce/)

