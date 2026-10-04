# Cuaderno de Adolfo · fitocardozo.com

Sitio personal bilingüe (ES/EN) con proyectos no profesionales: software, electrónica, música, aire libre, aprendizaje y más. Construido con Jekyll, el generador nativo de GitHub Pages.

## Publicar

En **Settings → Pages** del repositorio, elige *Deploy from a branch*, rama `main`, carpeta `/ (root)`. GitHub construye el sitio solo en cada push a `main` y lo sirve en <https://fitocardozo.com>.

## Añadir contenido

Cada pieza existe en dos archivos, uno por idioma, unidos por el mismo `ref` (así funciona el botón ES/EN).

**Un proyecto** → `_projects/es/<nombre>.md` y `_projects/en/<nombre>.md`:

```yaml
---
title: Nombre del proyecto
ref: nombre              # igual en ambos idiomas
permalink: /proyectos/nombre/     # en inglés: /en/projects/nombre/
area: maker              # software | maker | music | outdoor | learning | more
status: active           # active | paused | done | idea
year: 2026
order: 2                 # orden en las listas
summary: Una o dos frases.
repo: https://github.com/acardozos/...   # opcional
demo: https://...                         # opcional
stack: [Arduino, C++]
---
Texto en Markdown…
```

**Una entrada de bitácora** → `_posts/es/AAAA-MM-DD-titulo.md` y `_posts/en/AAAA-MM-DD-title.md` con `title`, `ref`, `permalink` (`/bitacora/...` o `/en/log/...`) y opcionalmente `area`.

**Foto, ubicación y enlaces** → `_data/profile.yml` (la foto va en `assets/img/`). **Áreas** → `_data/areas.yml`. **Textos de la interfaz** → `_data/i18n.yml`. **Colores y tipografía** → variables al inicio de `assets/css/main.css`.

## Probar en local

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```
