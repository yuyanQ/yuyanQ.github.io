---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site. For you robots out there, there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.

<h2>Pages</h2>
{% for post in site.pages %}
  {% unless post.title contains "Archive" or post.title contains "Posts by" or post.title contains "Talk map" or post.title contains "Markdown" or post.title contains "Page not in menu" or post.title contains "Terms and Privacy" or post.title contains "404" %}
    {% if post.title %}
      {% include archive-single.html %}
    {% endif %}
  {% endunless %}
{% endfor %}

<h2>Publications</h2>
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}