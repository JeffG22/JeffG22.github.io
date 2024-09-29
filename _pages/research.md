---
layout: archive
title: "Research"
titleWeb: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

{% if author.googlescholar %}
  You can also find my articles on <a href="{{author.googlescholar}}">my Google Scholar profile</a>.
{% endif %}

## Publications
{% for post in site.publications reversed %}
  {% include archive-single-pub.html %}
{% endfor %}

<!-- ## Preprints and Working Papers
{% for post in site.preprints reversed %}
  {% include archive-single-pub.html %}
{% endfor %} -->
