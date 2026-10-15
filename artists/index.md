---
layout: default
title: Artists
permalink: /artists/
---

# Artists

{% comment %}
  Collection index page.
  Lists the records in this collection and links to their individual pages.
  Sort records alphabetically to make browsing predictable as the archive grows.
{% endcomment %}
<ul>
  {% assign artists = site.artists | sort: "name" %}
  {% for artist in artists %}
    <li>
      <a href="{{ artist.url | relative_url }}">{{ artist.name }}</a>
    </li>
  {% endfor %}
</ul>