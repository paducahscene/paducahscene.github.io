---
layout: default
title: Releases
permalink: /releases/
---

# Releases

<ul>
  {% assign releases = site.releases | sort: "title" %}
  {% for release in releases %}
    <li>
      <a href="{{ release.url | relative_url }}">{{ release.title }}</a>
    </li>
  {% endfor %}
</ul>