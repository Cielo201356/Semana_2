# Semana 2

Proyecto base para la entrega de la semana 2, con documentación de auditoría, guía de desarrollo y preparación para despliegue en GitHub Pages.

## Objetivo

- Centralizar la documentación del proyecto.
- Registrar la auditoría y validaciones.
- Preparar el repositorio para publicar el sitio vía GitHub Pages.

## Estructura principal

- `index.html`: sitio principal.
- `styles.css`: estilos del sitio.
- `script.js`: comportamiento mínimo.
- `AUDITORIA.md`: documento de auditoría.
- `GUIA_DESARROLLADOR.md`: guía de trabajo para el equipo.
- `.github/workflows/deploy-pages.yml`: flujo de despliegue automático.

## Cómo ejecutar localmente

1. Descarga o clona el repositorio.
2. Abre la carpeta del proyecto.
3. Ejecuta un servidor local, por ejemplo:

```bash
python -m http.server 8000
```

4. Abre en el navegador la URL:

```text
http://localhost:8000
```

## Despliegue

El repositorio incluye un workflow de GitHub Actions para desplegar el sitio en GitHub Pages.

### Requisitos

- El repositorio debe estar en GitHub.
- La rama principal debe ser `main`.
- En GitHub, activar la opción de GitHub Pages con el origen de GitHub Actions.

## Estado

- Sitio estático preparado.
- Auditoría documentada.
- Guía del desarrollador creada.
- Workflow de despliegue listo.
