---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  <h2 class="archive__item-title" itemprop="headline">
    {{ post.title }}
  </h2>
  <!-- citation and icon code -->
  <p>
  {% if post.citation %}
    {{ post.citation }}
  {% endif %}
  <br>
  {% if post.venue %}
    {{ post.venue }}, {{ post.year }}
  {% endif %}
  <br>
  {% if post.authors %}
    {{ post.authors }}
  {% endif %}
  <br>
  {% if post.link %}
    <a href="{{ post.link }}"><i class="fas fa-fw fa-link zoom" aria-hidden="true"></i></a>
  {% endif %}
  {% if post.paperurl %}
    <a href="{{ post.paperurl }}"><i class="fas fa-fw fa-file-pdf zoom" aria-hidden="true"></i></a>
  {% endif %}
  {% if post.code %}
    <a href="{{ post.code }}"><i class="fas fa-fw fa-code zoom" aria-hidden="true"></i></a>
  {% endif %}
  {% if post.github %}
    <a href="{{ post.github }}"><i class="fab fa-fw fa-github zoom" aria-hidden="true"></i></a>
  {% endif %}
  </p>
{% endfor %}