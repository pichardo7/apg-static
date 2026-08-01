# apg-static

Sitio personal (apg.dev): nginx sirviendo HTML estático dentro de un contenedor Docker en el homelab.

- `docker-compose.yml` — define el contenedor `apg-static` (nginx:alpine, puerto 8091, sirve `./html`).
- `html/` — el sitio: `index.html`, `proyectos.html`, `codigo.html`, `selfhosted.html`, `styles.css`, `favicon.svg`.

Este commit inicial es un mirror del contenido que corre en producción. Los assets binarios del sitio (`favicon-32.png`, `apple-touch-icon.png`, `og-image.png`) no se incluyeron todavía — quedan pendientes de subir en un commit aparte.
