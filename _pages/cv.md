---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
  <ul>
  {% for post in site.education %}
    <p> {{ post.title }}, {{ post.university }} </p>
  {% endfor %}
  </ul>

Work Experience
======
  <ul>
  {% for post in site.industry %}
    <p> - {{ post.title }}, {{ post.company }} </p>
  {% endfor %}
  </ul>

Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>
  {% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}
  </ul>
  