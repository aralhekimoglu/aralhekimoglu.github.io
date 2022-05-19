---
layout: archive
title: "Education"
permalink: /education/
author_profile: true
---

{% include base_path %}

{% for post in site.education reversed %}
  <h2 class="archive__item-title" itemprop="headline">
    {{ post.title }} &#9737; [{{ post.dates }}]
  </h2>
  <b> {{ post.university }} </b>, {{ post.location }} <br>
  <p class="archive__item-excerpt" itemprop="description">
    <p>{{ post.excerpt | markdownify | remove: '<p>' | remove: '</p>' }}</p>
  </p>
{% endfor %}
