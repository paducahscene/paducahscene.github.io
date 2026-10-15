---
layout: default
title: Locations
permalink: /locations/
---

# Locations

{% comment %}
  Collection index page.
  Lists the records in this collection and links to their individual pages.
  Sort records alphabetically to make browsing predictable as the archive grows.
{% endcomment %}
<ul>
  {% assign locations = site.locations | sort: "name" %}
  {% for location in locations %}
    <li>
      <a href="{{ location.url | relative_url }}">{{ location.name }}</a>
    </li>
  {% endfor %}
</ul>