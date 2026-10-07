# Guía del desarrollador

## Propósito

Esta guía describe cómo trabajar con el proyecto, hacer cambios y preparar el despliegue en GitHub Pages.

## Requisitos locales

- Git
- Navegador web
- Python 3 (opcional para servir archivos localmente)

## Clonar el repositorio

```bash
git clone https://github.com/Cielo201356/Semana_2.git
cd Semana_2
```

## Ejecutar el proyecto localmente

### Opción 1: Python

```bash
python -m http.server 8000
```

Luego abrir:

```text
http://localhost:8000
```

### Opción 2: abrir directamente el HTML

Se puede abrir el archivo `index.html` en el navegador, aunque el servidor local es mejor para validar más aspectos del sitio.

## Flujo de trabajo recomendado

1. Crear una rama para cada tarea.
2. Hacer cambios mínimos y documentarlos.
3. Revisar que la página se visualiza correctamente.
4. Hacer commit con mensajes claros.
5. Hacer push y comprobar despliegue.

## Ejemplo de flujo

```bash
git checkout -b feature/nueva-seccion
git status
git add .
git commit -m "Añadir sección inicial del proyecto"
git push origin feature/nueva-seccion
```

## Despliegue en GitHub Pages

El repositorio incluye un workflow automatizado en:

```text
.github/workflows/deploy-pages.yml
```

### Pasos

1. Subir el repositorio a GitHub.
2. En la configuración del repositorio, ir a `Settings > Pages`.
3. Elegir `GitHub Actions` como origen.
4. Confirmar que el workflow se dispara con el push a `main` o ejecutarlo manualmente desde `Actions > Deploy static site to GitHub Pages > Run workflow`.
5. En `Actions`, abrir la ejecución más reciente y verificar que el job `deploy` finalizó con estado `success`.
6. Abrir el sitio publicado y comprobar que responde correctamente:

   <https://cielo201356.github.io/Semana_2/>

### Estado actual

El despliegue inicial se completó correctamente. La ejecución [#4](https://github.com/Cielo201356/Semana_2/actions/runs/37659315864), correspondiente al commit `74f696d` de `main`, terminó con éxito. El sitio publicado responde con HTTP 200.

## Buenas prácticas

- Mantener el README actualizado.
- Registrar cambios importantes en la auditoría.
- Hacer commits descriptivos.
- Validar el sitio antes de publicar.

## Soporte

Si hay cambios de estructura o documentación, actualizar también este archivo y `AUDITORIA.md` para mantenerse alineados con el proyecto.
