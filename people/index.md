---
layout: default
title: People
permalink: /people/
---

# People

<ul>
  {% assign people = site.people | sort: "name" %}
  {% for person in people %}
    <li>
      <a href="{{ person.url | relative_url }}">{{ person.name }}</a>
    </li>
  {% endfor %}
</ul>