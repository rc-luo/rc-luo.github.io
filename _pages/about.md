---
permalink: /
title: "About me"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I hold a bachelor degree of computer science in [Zhejiang University](https://www.zju.edu.cn/english/). I'm interested in mathematical optimziation, convex analysis, statistics, and stochastic processes. I enjoy the research work as a combination of mathematical beauty and formal rigor.


<!-- <span style="color:#58afe4">*Highlight.*
I am constantly seeking internship opportunities or other research collaborations. Please feel free to reach out via <a href="mailto:{{site.author.email}}">email</a> ;)</span> -->
<span style="color:#58afe4">*Highlight.*
I'm re-applying and actively looking for a phd position right now! ;)</span>


My research
======
My research interests include but are not limited to:
  - Mathematical optimization,
  - Convex analysis,
  - Statistics & stochastic processes.


Featured publications 
======
(You may see the full list [here](/publications).)
  <ul>{% for post in site.publications reversed %}
    {% if post.featured == true %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

Selected posts
======
(You may see the full list [here](/year-archive).)
  <ul><h1 class="archive__subtitle">Pinned</h1>
  {% for post in site.posts %}
    {% if post.pinned == true %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

  <ul>{% capture last_year %}'None'{% endcapture %}
  {% for post in site.posts %}
    {% if post.pinned == false %}
      <h1 class="archive__subtitle">Recent</h1>
      {% capture last_year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% break %}
    {% endif %}
  {% endfor %}
  
  {% for post in site.posts %}
    {% if post.pinned == false %}
      {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% if year == last_year %}
        {% include archive-single-cv.html %}
      {% endif %}
    {% endif %}
  {% endfor %}</ul>