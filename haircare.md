---
layout: page
title: HairCare
---

<div class="related">
  <ul class="related-posts">
    {% for post in site.categories.haircare limit:10 %}
      <li>
        <h3>
          <a href="{{ post.url }}">
            {% for tags in post.tags %}
              <h6 class="post-tags">{{ post.tags }}</h6>
            {% unless forloop.last %}{% endunless %}
            {% endfor %}{{ post.title }}
          </a>
        </h3>
      </li>
    {% endfor %}
  </ul>
</div>
