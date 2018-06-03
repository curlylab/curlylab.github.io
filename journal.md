---
layout: page
title: Journal
---

<div class="posts">
  {% for post in site.categories.journal limit:6 %}
  <div class="post">
    {% for tags in post.tags %}
      <h3 class="post-tags">{{ post.tags }}</h3>
    {% unless forloop.last %}{% endunless %}
    {% endfor %}
    <h1 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>
    {{ post.excerpt }}
      <a class="post-more" href="{{ post.url }}">
        Read more
      </a>
  </div>
  {% endfor %}
</div>
