---
layout: page
title: Archivo Literario
---

<div class="archive-intro">
  <p>Aquí encontrarás todos mis escritos organizados por categorías. Sientete libre de explorar mi colección literaria.</p>
</div>

<div class="archive-section">
  {% for tag in site.tags %}
    <h2 id="{{ tag[0] | slugify }}">{{ tag[0] }}</h2>
    <ul class="archive-list">
      {% for post in tag[1] %}
        <li>
          <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
          <span class="post-date">{{ post.date | date: "%d %B %Y" }}</span>
          {% if post.excerpt %}
            <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  {% endfor %}
</div>