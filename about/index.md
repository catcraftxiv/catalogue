---
layout: page
current: about
title: About
navigation: true
logo: 'assets/images/ghost.png'
class: page-template
subclass: 'post page'
---

Catcraft is consist of [pillow]({{ site.baseurl }}author/pillow/) and [Evie]({{ site.baseurl }}author/evie/) ^-^ If you need something, please do write **pillow39** at discord :>

**Every** of subscription rewards is custom made by us! :>

*This website is made to preview paid mods in one place! To see free mods in one place, please see <a href="https://www.xivmodarchive.com/user/111283" target="_blank">XIV Mod Archive profile</a> :>*

<details>
  <summary>Links to our things</summary>
{% for profile_page in site.data.profiles %}
<li><a href="{{ profile_page.link }}">{{ profile_page.name }}</a></li>
{% endfor %}
</details>

<a href="{{ site.baseurl }}rules/">See mod rules here!</a>