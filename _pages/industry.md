---
layout: archive
title: "Industry"
permalink: /industry/
author_profile: true
---

{% include base_path %}

{% for post in site.industry reversed %}
  <h2 class="archive__item-title" itemprop="headline">
    {{ post.title }} &#9679; {{ post.dates }}
  </h2>
  <b> {{ post.company }} </b>, {{ post.location }} <br>

  <p class="archive__item-excerpt" itemprop="description">
    <p>{{ post.excerpt | markdownify | remove: '<p>' | remove: '</p>' }}</p>
  </p>
{% endfor %}
