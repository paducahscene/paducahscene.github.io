---
layout: default
title: Artists
permalink: /artists/
---

# Artists

<ul>
  {% assign artists = site.artists | sort: "name" %}
  {% for artist in artists %}
    <li>
      <a href="{{ artist.url | relative_url }}">{{ artist.name }}</a>
    </li>
  {% endfor %}
</ul>