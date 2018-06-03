---
layout: page
title: HairCare
---

<div class="posts">
  {% for post in site.categories.haircare %}
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

    <span class="post-date">
      {% for category in post.categories %}
        #{{category}}
      {% unless forloop.last %}&nbsp;{% endunless %}
      {% endfor %}
    </span>

    {{ post.excerpt }}
      <a class="post-more" href="{{ post.url }}">
        Read more
      </a>
  </div>
  {% endfor %}
</div>
