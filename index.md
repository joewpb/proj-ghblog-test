---
title: Joe Blanco | Skills & Projects
description: Hermes Agent Skills Catalog
layout: default
permalink: /
---

Welcome to the Hermes Agent Skills Catalog &mdash; an index of all skills and projects built by me, Joe Blanco, powered by the Hermes agent framework and published via the ghblog-agent pipeline.

<div style="display:grid; grid-template-columns:repeat(auto-fill,minmax(280px,1fr)); gap:1rem;">
{% for p in site.pages %}
{% if p.title and p.url != "/" %}
<a class="skill-card" href="{{ p.url }}" style="text-decoration:none; color:inherit; display:block;">
  <h3 style="margin:0 0 .25rem;">{{ p.title }}</h3>
  <small>{{ p.date | date: "%b %d, %Y" }}</small>
  <p style="margin:.5rem 0 0; font-size:.9rem;">{{ p.description }}</p>
</a>
{% endif %}
{% endfor %}
</div>