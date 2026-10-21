# Yovany Ads · Portafolio

Portafolio de **Yovany** — Senior Media Buyer y Trafficker Digital. Una sola página estática (`index.html`) en formato "película": seis escenas a pantalla completa, casos interactivos, mercados y la tabla completa de cuentas de Meta Ads.

## Estructura

```
index.html                     # el sitio completo (HTML + CSS + JS inline, sin dependencias)
.github/workflows/pages.yml    # despliegue automático a GitHub Pages
.nojekyll                      # sirve los archivos tal cual, sin Jekyll
```

## Ver en local

```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

## Publicar en GitHub Pages

1. Fusiona esta rama en `main`.
2. En el repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. Cada push a `main` despliega el sitio en `https://yovanyads.github.io/portfolio/`.

## Actualizar los números

Los datos de las cuentas están en el objeto `D` dentro del `<script>` final de `index.html` (`rows` por cuenta y `tot` con los totales). Las cifras de las escenas (67,8 M impresiones, 132.467 leads, etc.) están escritas en el HTML de cada sección.
