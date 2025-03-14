---
layout: home
title: Colección Literaria
---

# Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vitae augue erat. Nulla at neque quis erat congue convallis. Proin ultrices ullamcorper quam, sit amet elementum nisl maximus sed. Suspendisse dignissim dapibus tortor et faucibus. Phasellus in mauris aliquam, lacinia purus sit amet, scelerisque velit. Nunc nec tortor molestie est accumsan laoreet at non justo. Suspendisse dapibus ut purus sit amet ultricies. Vestibulum a urna odio. Donec vel est efficitur, euismod massa vel, feugiat lectus. Phasellus tincidunt pulvinar est, fringilla vehicula felis aliquam eget. Sed fermentum dictum sem, nec iaculis elit feugiat consectetur. Aenean ultricies finibus euismod. Nunc eu leo varius, venenatis metus nec, posuere eros. 

## is to have it, simply because it is pain

<div class="featured-works">
  {% for post in site.posts limit:3 %}
    <div class="featured-work">
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
      <p class="meta">{{ post.date | date: "%B %d, %Y" }} • {% if post.genre %}{{ post.genre }}{% else %}Uncategorized{% endif %}</p>
      <p class="excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read more →</a>
    </div>
  {% endfor %}
</div>