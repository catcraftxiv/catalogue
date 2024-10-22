---
layout: page
current: about
title: Filters
navigation: true
logo: 'assets/images/ghost.png'
class: page-template
subclass: 'post page'
---

## Collections:

#### [subscription]({{ site.baseurl }}tag/subscription)
Monthly rewards for patreon/boosty. When you are subscribed, you have access to all of these :>
#### [shop]({{ site.baseurl }}tag/shop)
Mods that only can be bought in shop

*To see free mods, visit [XIV Mod Archive page](https://www.xivmodarchive.com/user/111283)*

## Tags:

{% for tag in site.data.tags %}
<li><a href="{{ site.baseurl }}tag/{{ tag[1].name }}">{{ tag[1].name }}</a></li>
{% endfor %}