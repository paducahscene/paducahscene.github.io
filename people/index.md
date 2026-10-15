---
layout: default
title: People
permalink: /people/
---

# People

{% comment %}
  Collection index page.
  Lists the records in this collection and links to their individual pages.
  Sort records alphabetically to make browsing predictable as the archive grows.
{% endcomment %}
<ul>
  {% assign people = site.people | sort: "name" %}
  {% for person in people %}
    <li>
      <a href="{{ person.url | relative_url }}">{{ person.name }}</a>
    </li>
  {% endfor %}
</ul>