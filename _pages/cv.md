---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Publications
======
  <ul>
  {% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}
  </ul>
  
Work Experience
======
  <ul>
  {% for post in site.industry %}
    <p> * {{ post.title }}, {{ post.company }} </p>
  {% endfor %}
  </ul>

Education
======
  <ul>
  {% for post in site.education %}
    <p> {{ post.title }}, {{ post.university }} </p>
  {% endfor %}
  </ul>

Skills
======
*Coding Languages:* Python, C++, MySQL, HTML, CSS, JavaScript
*Frameworks and Libraries:* PyTorch, TensorFlow, OpenCV, TensorRT, Keras, scikit-learn