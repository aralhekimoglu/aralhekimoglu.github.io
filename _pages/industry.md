---
layout: archive
title: "Industry"
permalink: /industry/
author_profile: true
---

{% include base_path %}

{% for post in site.industry reversed %}
  <h2 class="archive__item-title" itemprop="headline">
    {{ post.title }}
  </h2>
  <b> {{ post.company }} </b> , {{ post.location }}
  [{{ post.dates }}]
{% endfor %}
