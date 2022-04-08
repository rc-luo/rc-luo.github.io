---
permalink: /
title: "About Me"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am currently an undergraduate student in Zhejiang University, majoring in computer science. 


My research
======
My research interest lies broadly in machine learning and optimization, and, more particularly, in:
  - Distributed optimization,
  - Statistical learning,
  - Machine learning for real-world scenarios (*e.g.*, medical image analysis).
  
<span style="color:#58afe4">Highlight!</span>
I am constantly seeking internship opportunities or other research collaborations. Feel free to reach out via <a href="mailto:{{site.author.email}}">email</a> ;)


Featured publications 
======
  (You may see the full list [here](/publications).)
  <ul>{% for post in site.publications reversed %}
    {% if post.featured == true %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

Recent posts
======
  <ul>{% for post in site.posts limit: 5 reversed %}
    {% include archive-single.html %}
  {% endfor %}</ul>
