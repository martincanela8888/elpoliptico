## layout: home title: Devaneos

Voy a publicar cuentos (en general fantásticos de toda rama), poemas, ensayos y fragmentos. Sientanse libres de leer, comentar y compartir lo que deseen. Cualquier comentario, crítico o laudatorio es enormemente agradecido. Planeo publicar con cierta regularidad, aunque no se esperen milagros, ya que en breve volveré a ser esclavo de la facultad (Puan)  

"El gran monstruo del juego esclaviza a tu madre, ¡y se llama Jugón!"-Homero Simpson

  
  

### \[{{ post.title\]({{ site.baseurl }}{{ post.url }})

{{ post.date | date: "%B %d, %Y" }} • {% if post.genre %}{{ post.genre }}{% else %}Uncategorized{% endif %}

{{ post.excerpt | strip\_html | truncatewords: 30 }}

\[Read more →\]({{ site.baseurl }}{{ post.url }})

{% endfor %} \[}}\]({{ site.baseurl }}{{ post.url }})