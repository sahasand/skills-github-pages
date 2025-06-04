---
layout: default
title: My Stories
---

<link rel="stylesheet" href="/assets/css/style.css">

<header>
  <h1>Welcome to My Stories</h1>
  <p>Thoughts, adventures and ideas.</p>
</header>

<main>
  <ul class="post-list">
    {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </li>
    {% endfor %}
  </ul>
</main>

<footer>
  &copy; {{ site.time | date: '%Y' }}
</footer>
