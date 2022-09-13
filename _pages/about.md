---
permalink: /
title: "About me"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am an (incoming) PhD student at [CISPA Helmholtz Center for Information Security](https://cispa.de/en/) starting at 2022 fall. Prior to that, I received my bachelor degree of computer science in [Zhejiang University](https://www.zju.edu.cn/english/).


My research
======
My research interests include but are not limited to:
  - Distributed optimization,
  - Statistical learning,
  - Privacy-preserving machine learning.

<span style="color:#58afe4">*Highlight.*
I am constantly seeking internship opportunities or other research collaborations. Feel free to reach out via <a href="mailto:{{site.author.email}}">email</a> ;)</span>


Featured publications 
======
  (You may see the full list [here](/publications).)
  <ul>{% for post in site.publications reversed %}
    {% if post.featured == true %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}</ul>

Selected posts
======
  (Pinned)
  <ul>{% for post in site.posts %}
    {% if post.pinned == true %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}</ul>

  (Recent)
  <ul>{% for post in site.posts limit:5 %}
    {% if post.pinned == false %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}</ul>