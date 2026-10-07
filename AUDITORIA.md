# Auditoría del proyecto Semana 2

## Fecha

2026-10-07

## Responsable

Equipo de desarrollo / auditoría interna

## Objetivo

Verificar el estado real del repositorio, la documentación y la preparación para la publicación del sitio en GitHub Pages.

## Alcance

- Revisión de la estructura del repositorio.
- Validación de la documentación del proyecto.
- Comprobación del estado de GitHub Pages y del workflow de despliegue.
- Registro de riesgos, observaciones y acciones pendientes.

## Resultados de auditoría

### 1. Estructura del repositorio

Se confirma la creación y sincronización de los archivos base del proyecto:

- `index.html`
- `styles.css`
- `script.js`
- `README.md`
- `AUDITORIA.md`
- `GUIA_DESARROLLADOR.md`
- `.github/workflows/deploy-pages.yml`

El repositorio ya está conectado al remoto de GitHub y el proyecto se encuentra subido en la rama `main`.

### 2. Documentación

Se dispone de una base documental adecuada:

- README general del proyecto.
- Documento de auditoría con estado y recomendaciones.
- Guía del desarrollador para trabajar y publicar el sitio.

### 3. Despliegue y GitHub Pages

Se preparó un workflow para GitHub Pages basado en GitHub Actions:

- `actions/checkout@v4`
- `actions/configure-pages@v5`
- `actions/upload-pages-artifact@v3`
- `actions/deploy-pages@v4`

Además, la opción de GitHub Pages quedó habilitada en el repositorio.

## Estado real verificado

### Cumplido

- El proyecto está subido a GitHub correctamente.
- El repositorio tiene la estructura base necesaria.
- La documentación del proyecto está creada.
- GitHub Pages está habilitado para el repositorio.
- El workflow de GitHub Actions completó correctamente el despliegue más reciente en `main` (ejecución [#4](https://github.com/Cielo201356/Semana_2/actions/runs/37659315864), commit `74f696d`).
- La URL pública de GitHub Pages responde con HTTP 200 y muestra el formulario publicado: <https://cielo201356.github.io/Semana_2/>.

### Pendientes

- No quedan pendientes para completar y verificar el despliegue inicial.

## Observaciones

### Riesgos y observaciones

- La primera ejecución del workflow falló; las ejecuciones posteriores completaron correctamente, incluida la ejecución más reciente (#4).
- El job `deploy` y sus pasos de configuración, carga del artefacto y publicación terminaron con éxito.

### Evidencia técnica

Se verificó que la ejecución más reciente del workflow concluyó con estado `success` para el commit `74f696d985455c29d5f8179accce85ba06acf8fd`. La URL <https://cielo201356.github.io/Semana_2/> devuelve HTTP 200 y presenta el formulario “Crear cuenta”.

## Recomendaciones

1. Consultar la [ejecución completada](https://github.com/Cielo201356/Semana_2/actions/runs/37659315864) en la pestaña `Actions` de GitHub.
2. Mantener la documentación actualizada con cada cambio relevante.

## Conclusión

El proyecto tiene una base correcta de repositorio, documentación y despliegue, y GitHub Pages está habilitado. El workflow completó correctamente la publicación y la página está accesible en su URL pública. La auditoría queda actualizada con esta verificación.
