---
layout: page
current: about
title: Testing Page
navigation: true
logo: 'assets/images/ghost.png'
class: page-template
subclass: 'post page'
---

Testing page :>

<li class="nav-home" role="menuitem"><a href="https://www.xivmodarchive.com/user/111283" target="_blank">XMA (manual)</a></li>
<li class="nav-home" role="menuitem"><a href="{{ site.data.profiles[XMA].link }}" target="_blank">XMA (from profiles.yml)</a></li>


{% for profile_page in site.data.profiles %}
{% if profile_page.frontpage %}
<li class="nav-home" role="menuitem"><a href="{{ profile_page.link }}" target="_blank">{{ profile_page.name }}</a></li>
{% endif %}
{% endfor %}