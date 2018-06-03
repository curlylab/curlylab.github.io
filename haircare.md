---
layout: page
title: HairCare
---

{% for post in site.categories.haircare %}
  <article class="post">
    <h2 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </h2>
  </article>
{% endfor %}
