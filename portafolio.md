---
layout: page
title: Portafolio creativo
permalink: /portafolio/
---

Soy ilustradora y científica. Uso la ilustración como puente entre la investigación y las personas: retratos de científicas, diseños inspirados en la vida microscópica y la naturaleza, y proyectos de divulgación junto a [Microbios](https://microbiosdigital.wordpress.com/).

{% assign categorias = site.data.portafolio | map: "categoria" | uniq %}
{% for cat in categorias %}
## {{ cat }}

<div class="galeria">
{% for obra in site.data.portafolio %}{% if obra.categoria == cat %}
{% if obra.imagen contains '://' %}{% assign src = obra.imagen %}{% else %}{% assign src = obra.imagen | prepend: '/' | prepend: site.baseurl %}{% endif %}
{% if obra.enlace %}{% assign destino = obra.enlace %}{% else %}{% assign destino = src %}{% endif %}
<figure class="obra">
<a href="{{ destino }}" target="_blank" rel="noopener">
<img src="{{ src }}" alt="{{ obra.titulo }}" loading="lazy">
</a>
<figcaption>
<strong>{{ obra.titulo }}</strong>{% if obra.anio %} · {{ obra.anio }}{% endif %}
{% if obra.tecnica %}<span class="tecnica">{{ obra.tecnica }}</span>{% endif %}
{% if obra.descripcion %}<span class="descripcion">{{ obra.descripcion }}</span>{% endif %}
</figcaption>
</figure>
{% endif %}{% endfor %}
</div>
{% endfor %}

## Actividades y trayectoria como ilustradora

- **2026** — Coordinación y dirección creativa de la quinta edición del *Calendario de Mujeres Ecuatorianas en Ciencias* ("Estamos aquí"), con el apoyo de la Cooperación Alemana en Ecuador y GENIA. [Ver calendario](https://microbiosdigital.wordpress.com/calendario-de-mujeres-ecuatorianas-en-ciencias-2026/)
- **2026** — Organizadora del *1er Concurso Arte, Ciencia y Mujeres: "La ciencia también se imagina, se dibuja"*, con el IRD en Ecuador (julio). [Ver anuncio](https://www.facebook.com/IRDenAmericaLatina/posts/ecuador-concurso-arte-ciencia-y-mujeres-la-ciencia-tambi%C3%A9n-se-imagina-se-dibuja-/1375981504572585/)
- **Juego de memoria** — Asistente y diseñadora de un juego de memoria de divulgación científica. [Ver video](https://www.youtube.com/watch?v=rqhlW01OdSQ&t=37s)
- **2022 – 2025** — Ilustración y línea editorial del *Calendario de Mujeres Ecuatorianas en Ciencias*, iniciativa de la Red Ecuatoriana de Mujeres Científicas (REMCI) y Microbios.
- **2022** — Ilustradora del primer *Calendario de Mujeres Ecuatorianas en Ciencias*, lanzado el 11 de febrero por el Día Internacional de la Mujer y la Niña en la Ciencia. Cobertura en [El Comercio](https://www.elcomercio.com/sociedad/ecuador-primer-calendario-mujeres-ciencia/) y Teleamazonas.
- **2021 – presente** — Diseño de portadas para las libretas de ciencia de Microbios. [Ver tienda](https://microbiosdigital.wordpress.com/tienda/)

¿Te interesa un encargo o colaboración? Escríbeme por [Instagram](https://www.instagram.com/ajchavez94) o a [andrea.chavezpacheco@ugent.be](mailto:andrea.chavezpacheco@ugent.be).
