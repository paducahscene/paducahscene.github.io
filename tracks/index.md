---
layout: default
title: Tracks
permalink: /tracks/
---

# Tracks

{% comment %}
  Collection index page.
  Lists the records in this collection and links to their individual pages.
  Sort records alphabetically to make browsing predictable as the archive grows.
{% endcomment %}
<ul>
  {% assign tracks = site.tracks | sort: "title" %}
  {% for track in tracks %}
    <li>
      <a href="{{ track.url | relative_url }}">{{ track.title }}</a>
    </li>
  {% endfor %}
</ul>