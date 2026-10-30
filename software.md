---
layout: default
title: Software
---
# Software

Open-source tools I have developed or contributed to.

<ul class="publications">
{% for s in site.data.software %}
  <li>
    <strong>{% if s.url %}<a href="{{ s.url }}">{{ s.name }}</a>{% else %}{{ s.name }}{% endif %}</strong> · {{ s.role }} · {{ s.years }}<br>
    {{ s.description }}
  </li>
{% endfor %}
</ul>
