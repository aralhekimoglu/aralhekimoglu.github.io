---
layout: archive
title: "Education"
permalink: /education/
author_profile: true
---

{% include base_path %}

{% for post in site.education reversed %}
  <h2 class="archive__item-title" itemprop="headline">
    {{ post.title }}
  </h2>
  <b> {{ post.university }} </b>, {{ post.location }} <br>
  {{ post.dates }}
{% endfor %}
