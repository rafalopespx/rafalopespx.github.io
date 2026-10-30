---
layout: default
title: Publications
---
# Publications

<p class="legend">* first, co-first or senior author; ° corresponding author. Publications up to 2022 appear under the name R. L. P. da Silva.</p>

## Preprints and manuscripts under review

<ul class="publications">
{% assign preprints = site.data.publications | where: "type", "preprint" %}
{% for p in preprints %}
  <li>
    <strong>{{ p.title }}</strong><br>
    {{ p.authors | replace: "Lopes R", "<strong>Lopes R</strong>" | replace: "da Silva RLP", "<strong>da Silva RLP</strong>" }}<br>
    <em>{{ p.venue }}</em>{% if p.year %} ({{ p.year }}){% endif %}{% if p.doi %} · <a href="https://doi.org/{{ p.doi }}">DOI</a>{% endif %}
  </li>
{% endfor %}
</ul>

## Peer-reviewed articles

<ul class="publications">
{% assign articles = site.data.publications | where: "type", "article" %}
{% for p in articles %}
  <li>
    <strong>{{ p.title }}</strong><br>
    {{ p.authors | replace: "Lopes R", "<strong>Lopes R</strong>" | replace: "da Silva RLP", "<strong>da Silva RLP</strong>" }}<br>
    <em>{{ p.venue }}</em>{% if p.year %} ({{ p.year }}){% endif %}{% if p.doi %} · <a href="https://doi.org/{{ p.doi }}">DOI</a>{% endif %}
  </li>
{% endfor %}
</ul>

## Conference abstracts

<ul class="publications">
{% assign abstracts = site.data.publications | where: "type", "abstract" %}
{% for p in abstracts %}
  <li>
    <strong>{{ p.title }}</strong><br>
    {{ p.authors | replace: "Lopes R", "<strong>Lopes R</strong>" | replace: "da Silva RLP", "<strong>da Silva RLP</strong>" }}<br>
    <em>{{ p.venue }}</em>{% if p.year %} ({{ p.year }}){% endif %}
  </li>
{% endfor %}
</ul>
