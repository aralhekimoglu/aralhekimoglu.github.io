---
layout: archive
title: "Industry"
permalink: /industry/
author_profile: true
---

{% include base_path %}

{% for post in site.industry reversed %}
  <h2 class="archive__item-title" itemprop="headline">
    {{ post.company }}, {{ post.location }}
  </h2>
  <b> {{ post.title }} </b> {{ post.dates }}
{% endfor %}
