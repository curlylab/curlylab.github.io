---
layout: page
title: HairCare
---

{% for post in site.categories.journal %}
  <article class="post">
    <small><h1 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </h1></small>
  </article>
{% endfor %}
