---
layout: archive
title: "Education"
permalink: /education/
author_profile: true
---

{% include base_path %}

{% for post in site.education reversed %}
  <p> {{ post.title }}, { post.university }} </p>
{% endfor %}
