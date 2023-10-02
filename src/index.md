---
layout: base.njk
title: Mi Blog Sam
---

# {{ title }}



[Acerca]({{ '/acerca' | url }})

## Artículos 

### Categoría Videojuegos Favoritos

{% for videojuego in collections.videojuegos %}

- [{{videojuego.data.title}}]({{ videojuego.url | url }})

{% endfor %}

### Categoria Series Favoritas

{% for serie in collections.series %}

- [{{serie.data.title}}]({{ serie.url | url }})

{% endfor %}

### Categoria Peliculas Favoritas

{% for pelicula in collections.peliculas %}

- [{{pelicula.data.title}}]({{ pelicula.url | url }})

{% endfor %}
