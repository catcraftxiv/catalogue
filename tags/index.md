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

###### [subscription]({{ site.baseurl }}tag/subscription)
Monthly rewards for patreon/boosty. When you are subscribed, you have access to all of these :>
###### [shop]({{ site.baseurl }}tag/shop)
Mods that only can be bought in shop
###### <a href="https://www.xivmodarchive.com/user/111283" target="_blank">Free</a>
Free mods, gathered on XIV Mod Archive page

## Tags:

{% for tag in site.data.tags %}
<li><a href="{{ site.baseurl }}tag/{{ tag[1].name }}">{{ tag[1].name }}</a></li>
{% endfor %}