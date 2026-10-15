---
layout: default
title: Releases
permalink: /releases/
---

# Releases

{% comment %}
  Collection index page.
  Lists the records in this collection and links to their individual pages.
  Sort records alphabetically to make browsing predictable as the archive grows.
{% endcomment %}
<ul>
  {% assign releases = site.releases | sort: "title" %}
  {% for release in releases %}
    <li>
      <a href="{{ release.url | relative_url }}">{{ release.title }}</a>
    </li>
  {% endfor %}
</ul>