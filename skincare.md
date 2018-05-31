---
layout: page
title: SkinCare
---

{% for post in site.categories.skincare %}
  <article class="post">
    <h1 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </h1>
    {{ post.content }}
  </article>
{% endfor %}
