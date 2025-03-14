---
layout: default
current: home
class: 'home-template'
navigation: True
permalink: b/
---

<style>
  .homepage-info {
	box-shadow: rgba(0, 0, 0, 0.16) 0px 3px 6px, rgba(0, 0, 0, 0.23) 0px 3px 6px;
	background-color: rgb(255, 255, 255);
}
</style>

<!-- < default -->
<!-- The tag above means: insert everything in this file
into the {body} of the default.hbs template -->

<!-- The big featured header, it uses blog cover image as a BG if available -->
<header class="site-header outer {% if page.cover or site.cover %}" style="background-image:  url({{ site.baseurl }}{% if page.cover %}{{ page.cover }}{% elsif site.cover %}{{ site.cover }}{% endif %}) {% else %}no-cover{% endif %}" markdown="0">
    <div class="inner" markdown="0">
        <div class="site-header-content" markdown="0">
            <h1 class="site-title" markdown="0">
                {% if site.logo %}
                    <img class="site-logo" src="{{ site.baseurl }}{{ site.logo }}" alt="{{ site.title }}"/>
                {% else %}
                    {{ site.title }}
                {% endif %}
            </h1>
            <h2 class="site-description">{% if page.description %}{{ page.description }}{% else %}{{ site.description }}{% endif %} markdown="0"</h2>
        </div>
        {% include site-nav.html %}
    </div>
</header>

<!-- The main content area -->
<main id="site-main" class="site-main outer" role="main" markdown="0">
    <div class="inner" markdown="0">
        <div class="post-feed" markdown="0">
		    <section class="post-full-content" markdown="0">
                <div class="kg-card-markdown" markdown="1">
                    {% include homepage.md %}
                </div>             
            </section>
        </div>
    </div>
</main>
