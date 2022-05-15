---
layout: archive
title: "Industry"
permalink: /industry/
author_profile: true
---

{% include base_path %}

{% for post in site.industry reversed %}
  <p> {{ post.title }}, {{ post.company }} </p>
{% endfor %}
