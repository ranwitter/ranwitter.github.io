---
layout: page
title: Welcome
---

<h2>Welcome</h2>

<p>
  I'm Rangana. I write things about Technology.
  See also:
  <a href="https://www.linkedin.com/">LinkedIn</a>.
  <a href="https://github.com/ranwitter">GitHub</a>,
  <a href="https://twitter.com/ranwitter">Twitter</a>,
  <a href="https://github.com/ranwitter/dotfiles">my dotfiles</a>,
  and <a href="https://rangana.de">rangana.de</a>.
</p>

<h3>On this blog:</h3>

<ul class="my-4">
  {% for post in site.posts %}
    {% if post.draft != true %}
      <li class="my-3">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <br/><span class="text-secondary">{{ post.date | date_to_string }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>

