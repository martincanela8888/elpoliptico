---
layout: home
title: Devaneos
---

Voy a publicar cuentos (en general fantásticos de toda rama), poemas, ensayos y fragmentos. Sientanse libres de leer, comentar y compartir lo que deseen. Cualquier comentario, crítico o laudatorio es enormemente agradecido. Planeo publicar con cierta regularidad, aunque no se esperen milagros, ya que en breve volveré a ser esclavo de la facultad (Puan)

"El gran monstruo del juego esclaviza a tu madre, ¡y se llama Jugón!" - Homero Simpson

Lovecraftiano, Ballardiano, Marciano y coso

<div class="featured-works">
  {% for post in site.posts limit:3 %}
    <div class="featured-work">
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
      <p class="meta">{{ post.date | date: "%B %d, %Y" }} • {% if post.genre %}{{ post.genre }}{% else %}Uncategorized{% endif %}</p>
      <p class="excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Leer Más →</a>
    </div>
  {% endfor %}
</div>