# virela-legal

Sitio estático mínimo con las páginas legales de Virela, para la revisión de apps de TikTok for Developers (y de Meta si hace falta).

- `index.html`: qué es Virela, sus redes y enlaces visibles a privacidad y términos.
- `privacidad.html`: política de privacidad (español + inglés).
- `terminos.html`: términos del servicio (español + inglés).
- `callback.html`: redirect URI de Login Kit (muestra el `code` para canjearlo por token). URI a registrar: `https://bus-eng.github.io/virela-legal/callback.html`.
- `style.css`: estilo compartido.

## Publicar en GitHub Pages (lo aprueba Roberto)

1. Crear el repo público `bus-eng/virela-legal` en GitHub.
2. `git init && git add . && git commit -m "sitio legal" && git branch -M main`
3. `git remote add origin git@github.com:bus-eng/virela-legal.git && git push -u origin main`
4. En el repo: Settings > Pages > Source: Deploy from a branch > `main` / root.
5. URL resultante: `https://bus-eng.github.io/virela-legal/` (privacidad y términos cuelgan de ahí).

Sin build ni dependencias. Probar local: `python3 -m http.server` dentro de la carpeta.
