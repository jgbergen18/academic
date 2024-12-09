---
layout: default
title: posts
permalink: /posts/
---

<h3 class="mt-5 text-center">Monthly Posts</h3>
<div class="row g-4 mb-4">
  <div class="col-md-12">
    <ul class="list-unstyled">
      {% for post in site.posts %}
        <li class="mb-2">
          <a href="{{ site.github.url }}{{ post.url }}" class="text-decoration-none">
            <strong>{{ post.title }}</strong>
          </a>
          <span class="text-muted">- {{ post.date | date: "%B %-d, %Y" }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>
