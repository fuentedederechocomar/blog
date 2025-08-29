---
title: "Tesauro del sitio"
url: "/tesauro/"
---

Encuentra aquí un índice completo del contenido de nuestro sitio, organizado por categorías, temas, y etiquetas.

<p>
    Puedes usar este índice para encontrar el contenido que más te interesa, o simplemente para explorar los diferentes temas que cubrimos.
</p>

## Secciones

Aquí podrías listar las secciones principales de tu sitio.

---

## Categorías

<ul class="taxonomy-list">
    {{ range .Site.Taxonomies.categories.ByCount }}
    <li>
        <a href="{{ .Page.Permalink }}">{{ .Term }}</a>
        <span class="term-count">({{ .Count }})</span>
    </li>
    {{ end }}
</ul>

---

## Temas

<ul class="taxonomy-list">
    {{ range .Site.Taxonomies.topics.ByCount }}
    <li>
        <a href="{{ .Page.Permalink }}">{{ .Term }}</a>
        <span class="term-count">({{ .Count }})</span>
    </li>
    {{ end }}
</ul>

---

## Etiquetas

<ul class="taxonomy-list">
    {{ range .Site.Taxonomies.tags.ByCount }}
    <li>
        <a href="{{ .Page.Permalink }}">{{ .Term }}</a>
        <span class="term-count">({{ .Count }})</span>
    </li>
    {{ end }}
</ul>
