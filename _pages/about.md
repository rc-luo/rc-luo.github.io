---
permalink: /
title: "About me"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I hold a bachelor degree of computer science in [Zhejiang University](https://www.zju.edu.cn/english/). And I'm actively looking for a phd position right now. I have been working closely with [Dr. Sebastian U. Stich](http://sstich.ch) from [CISPA](https://cispa.de/en/) on optimization theory. Previously, I had worked as a research intern in HKU on federated learning, and Tencent ARC Lab on transfer learning. 
<!-- Please see [this post](/posts/2023/02/Shocked-by-the-bad-visa-decision) for the latest updates. -->
<!-- I am an (incoming) PhD student at [CISPA Helmholtz Center for Information Security](https://cispa.de/en/) starting at 2022 fall. Prior to that, I received my bachelor degree of computer science in [Zhejiang University](https://www.zju.edu.cn/english/). -->


My research
======
My research interests include but are not limited to:
  - Distributed optimization,
  - Statistical learning,
  - Privacy-preserving machine learning.

<span style="color:#58afe4">*Highlight.*
I am constantly seeking internship opportunities or other research collaborations. Please feel free to reach out via <a href="mailto:{{site.author.email}}">email</a> ;)</span>


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
  <ul><h2 class="archive__subtitle">Pinned</h2>
  {% for post in site.posts %}
    {% if post.pinned == true %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}</ul>

  <ul>{% capture last_year %}'None'{% endcapture %}
  {% for post in site.posts %}
    {% if post.pinned == false %}
      <h2 class="archive__subtitle">Recent</h2>
      {% capture last_year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% break %}
    {% endif %}
  {% endfor %}
  
  {% for post in site.posts %}
    {% if post.pinned == false %}
      {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% if year == last_year %}
        {% include archive-single.html %}
      {% endif %}
    {% endif %}
  {% endfor %}</ul>