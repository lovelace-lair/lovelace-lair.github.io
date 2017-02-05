---
layout: single
title: Members
---

{% for pauthor in site.data.authors %}
  {% assign author = pauthor[1] %}
  {% if author.status contains "current" %}
	{% include adalyte-profile.html %}
  {% endif %}
{% endfor %}

# Past Members

{% for pauthor in site.data.authors %}
  {% assign author = pauthor[1] %}
  {% if author.status contains "alumni" %}
	{% include adalyte-profile.html %}
  {% endif %}
{% endfor %}

# Founding Fathers

{% for pauthor in site.data.authors %}
  {% assign author = pauthor[1] %}
  {% if author.status contains "founder" %}
	{% include adalyte-profile.html %}
  {% endif %}
{% endfor %}

