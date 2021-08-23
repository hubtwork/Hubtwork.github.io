---
layout: main
title: Tech
main: true
---

<div class="loading-animation">

{% include tag-container.html %}

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'date' | reverse | where: 'type', 'tech' %}
{% for page in sorted %}
{% include post-list-item.html %}
{% endfor %}
</ul>
</div>