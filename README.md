# apg-static

Sitio personal (apg.dev): nginx sirviendo HTML estático dentro de un contenedor Docker en el homelab.

- `docker-compose.yml` — define el contenedor `apg-static` (nginx:alpine, puerto 8091, sirve `./html`).
- `html/` — el sitio: `index.html`, `proyectos.html`, `codigo.html`, `selfhosted.html`, `styles.css`, `favicon.svg`, `favicon-32.png`, `apple-touch-icon.png`, `og-image.png`.

Este repo es la fuente de verdad del sitio en producción. `$HOME/apg-static` en el host es un clon git (deploy key de solo lectura); el workflow de n8n "Desplegar apg-static" hace `git fetch` + `checkout -f main origin/main` + `docker compose up -d` para aplicar cambios.
