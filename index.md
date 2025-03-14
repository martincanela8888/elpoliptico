---
layout: home
title: Devaneos
---

<div class="hero-section">
  <h1>El Políptico</h1>
  <p>Un espacio para mis escritos: cuentos fantásticos, poemas, ensayos y fragmentos. Bienvenidos a mi mundo literario.</p>
</div>
<div class="container">
  <h2>Escritos:</h2>
  <div class="featured-works">
    {% for post in site.posts %}
      <div class="featured-work">
        <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
        <p class="meta">{{ post.date | date: "%d %B %Y" }} • {% if post.genre %}{{ post.genre }}{% else %}{% if post.tags %}{{ post.tags | first }}{% else %}Uncategorized{% endif %}{% endif %}</p>
        <p class="excerpt">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
        <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Leer Más →</a>
      </div>
    {% endfor %}
  </div>
  
  <div class="archive-link-container">
    <a href="{{ site.baseurl }}/archive" class="archive-link">Ver Archivo Completo →</a>
  </div>
</div>