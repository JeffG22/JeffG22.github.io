---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

{% if author.googlescholar %}
  You can also find my articles on <a href="{{author.googlescholar}}">my Google Scholar profile</a>.
{% endif %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}