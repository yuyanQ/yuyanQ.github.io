---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: false
---

A list of all the posts and pages found on the site. For you robots out there, there is an [XML version](/sitemap.xml) available for digesting as well.

## Pages

{% for post in site.pages %}
  {% unless post.title contains "Archive" or post.title contains "Posts by" or post.title contains "Talk map" or post.title contains "Markdown" or post.title contains "Page not in menu" or post.title contains "Terms and Privacy" %}
    {% if post.title %}
* [{{ post.title }}]({{ post.url }})
    {% endif %}
  {% endunless %}
{% endfor %}

## Publications
{% for post in site.publications reversed %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}

<!-- 暂时隐藏的内容
## Posts
{% for post in site.posts %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}

## Talks
{% for post in site.talks reversed %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}

## Teaching
{% for post in site.teaching reversed %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}
-->

