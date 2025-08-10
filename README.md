# Explicando-BB84

Sitio estático para explicar de forma clara el protocolo BB84 (distribución cuántica de claves).

> Nota original: Johelys te amo

## Estado del sitio
- Despliegue automático en GitHub Pages mediante GitHub Actions.
- La URL pública se mostrará en la salida del workflow tras el primer deploy.

## Estructura
- `index.html` en la raíz del repositorio.
- (Opcional) `assets/` para CSS, JS e imágenes.

## Desarrollo local
- Abre `index.html` directamente en tu navegador, o levanta un servidor local:

```bash
python3 -m http.server 8000
# luego visita http://localhost:8000
```

## Despliegue (GitHub Pages)
Este repositorio incluye un workflow en `/.github/workflows/pages.yml` que publica el contenido de la raíz.

- Cada push a la rama `main` dispara el deploy.
- No requiere configuración adicional si el repositorio es público. En repos privados, asegúrate de que tu plan permite GitHub Pages.
- Si es la primera vez, ve a Settings → Pages y selecciona "GitHub Actions" como fuente si no aparece automáticamente.

### URL de producción
- Tras el primer deploy, la URL aparece como "Page URL" en el job "Deploy to GitHub Pages" de la pestaña Actions.
- Convención habitual: `https://<usuario>.github.io/<repositorio>`.
- Para dominio personalizado, añade un archivo `CNAME` en la raíz con tu dominio.

## Siguientes pasos
- Añade `index.html` con el contenido del sitio.
- Si agregas CSS/JS/imágenes, colócalos en carpetas (por ejemplo `assets/`) y se publicarán automáticamente.
