# OmStack.dev · Portafolio de Christian Panche

Web estática (un solo `index.html`, sin dependencias ni compilación).

## Publicar en GitHub Pages

1. En GitHub crea un repositorio **público** llamado exactamente
   `christianpanche9-dot.github.io` (sin README).
2. En la terminal, dentro de esta carpeta:

   ```bash
   git init
   git add .
   git commit -m "Portafolio OmStack.dev"
   git branch -M main
   git remote add origin https://github.com/christianpanche9-dot/christianpanche9-dot.github.io.git
   git push -u origin main
   ```

   (También puedes arrastrar los archivos en GitHub con "Add file → Upload files".)
3. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   rama `main`, carpeta `/ (root)` → Save.
4. En 1–2 minutos estará en **https://christianpanche9-dot.github.io/**

## Actualizar
Cambia `index.html`, luego `git add . && git commit -m "Actualiza" && git push`.

## Más adelante: dominio propio (omstack.dev)
- Settings → Pages → Custom domain: `omstack.dev`.
- En tu proveedor de dominio crea registros A hacia 185.199.108.153, 185.199.109.153,
  185.199.110.153 y 185.199.111.153 (y CNAME `www` → `christianpanche9-dot.github.io`).
- Activa "Enforce HTTPS".
- Cambia en `index.html` las URLs de `og:url`, `og:image` y `canonical` al nuevo dominio.

## Archivos
- `index.html` — la web completa (estilos, scripts e imágenes incluidos).
- `og.png` — imagen que se muestra al compartir el enlace.
- `favicon.ico`, `favicon-32.png`, `apple-touch-icon.png` — iconos.
- `.nojekyll` — evita que GitHub procese la carpeta.
- `404.html` — redirige a la portada.
