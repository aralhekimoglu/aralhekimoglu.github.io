---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<iframe src="/files/CV.pdf" width="100%" height="500" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>

You can download a PDF copy of my CV [here](/files/CV.pdf).

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
  {% for post in site.industry reversed %}
    <li> {{ post.title }}, {{ post.company }} </li>
  {% endfor %}
  </ul>

Education
======
  <ul>
  {% for post in site.education reversed %}
    <li> {{ post.title }}, {{ post.university }} </li>
  {% endfor %}
  </ul>

Skills
======
* *Coding Languages:* Python, C++, MySQL, HTML, CSS, JavaScript
* *Frameworks and Libraries:* PyTorch, TensorFlow, OpenCV, TensorRT, Keras, scikit-learn