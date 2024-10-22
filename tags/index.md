---
layout: page
current: about
title: Tags
navigation: true
logo: 'assets/images/ghost.png'
class: page-template
subclass: 'post page'
---

{% for tag in site.data.tags %}
<li><a href="{{ site.baseurl }}tag/{{ tag.name }}">{{ tag.name }}</a></li>
{% endfor %}