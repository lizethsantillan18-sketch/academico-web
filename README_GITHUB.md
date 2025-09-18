
# Publicar en GitHub Pages — Sitio Estático (Firebase listo)

## Pasos
1) Crea un repo en GitHub (por ejemplo `academico-web`) y súbelo con **Add file → Upload files**.
   - Sube **index.html** y **healthcheck.html** (ambos vienen en este ZIP).
2) Ve a **Settings → Pages**.
3) En **Build and deployment** selecciona:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / **Folder:** `/` (root)
4) Guarda. En 1–2 minutos verás la URL: `https://TU-USUARIO.github.io/academico-web/`

## Firebase Auth
- En **Authentication → Settings → Authorized domains** agrega tu dominio de GitHub Pages:
  `TU-USUARIO.github.io`

## Pruebas
- Abre `/healthcheck.html` en tu dominio para verificar Auth + Firestore.
- Si dice `auth/unauthorized-domain`, te falta autorizar el dominio.
- Si dice `insufficient permissions`, te falta **publicar** las **Rules** en Firestore.
