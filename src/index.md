---
layout: base.njk
title: Mis peliculas,series y videojuegos que mas juego. 
---

# {{ title }}

Soy Hector Otero Caballero y aqui expondre mis series y peliculas favoritas. 

[Acerca de mi]({{ '/acerca' | url }})

## Artículos de mi Blog

### Categoría Peliculas

{% for pelicula in collections.pelicula %}

- [{{pelicula.data.title}}]({{ pelicula.url | url }})

{% endfor %}

### Categoria Series

{% for serie in collections.series %}

- [{{serie.data.title}}]({{ serie.url | url }})

{% endfor %}

### Categoria Videojuegos

{% for videojuego in collections.videojuego %}

- [{{videojuego.data.title}}]({{ videojuego.url | url }})

{% endfor %}