---
layout: page
title: Alumni
icon: fas fa-user-graduate
order: 5
permalink: /alumni/
---

<h2>Our Alumni</h2>

<ul>
  {% for person in site.alumni %}
    <li>
      <a href="{{ person.url | relative_url }}">
        <strong>{{ person.title }}</strong>
      </a><br>
      {{ person.batch }} — {{ person.position }}
    </li>
  {% endfor %}
</ul>
