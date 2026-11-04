# Laboratorio de Prácticas Ágiles – SENATI

Aplicación web del curso **Gestión de Proyectos de Software** (Semana 12) usada como proyecto central del laboratorio de prácticas ágiles con GitHub.

Está construida solo con **HTML5 + Bootstrap 5.3 + CSS + JavaScript**, sin dependencias locales ni proceso de compilación.

## Contenido del proyecto

| Archivo      | Descripción                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `index.html` | Página principal con las 3 secciones (Fundamentos, Guía y Tablero Kanban).    |
| `script.js`  | Navegación entre secciones y lógica del tablero Kanban (crear, mover, borrar).|
| `styles.css` | Estilos propios complementarios a Bootstrap.                                  |

## Cómo usar la aplicación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/<usuario>/develop_central.git
   cd develop_central
   ```

2. Abre `index.html` en el navegador (doble clic) o sirve la carpeta con un servidor local:

   ```bash
   python -m http.server 8000
   ```

3. Secciones disponibles:
   - **1. Fundamentos Ágiles**: Scrum, Kanban, XP y el Manifiesto Ágil.
   - **2. Guía de Laboratorio (GitHub)**: pasos del flujo de trabajo.
   - **3. Tablero Kanban Interactivo**: agrega tareas con el botón *Nueva Tarea*, muévelas entre *Por Hacer / En Proceso / Completado* y elimínalas.

> Las tareas del tablero se guardan en memoria: al recargar la página se restablecen las tareas de ejemplo.

## Flujo de trabajo ágil del equipo

```
Issue (User Story) → rama feature → Pull Request → revisión/Approve → merge a develop
```

- Todos los cambios sobre `index.html`, `script.js` y `styles.css` llegan a la rama `develop` del repositorio central **únicamente** mediante Pull Request aprobado.
- Cada integrante trabaja sobre su fork `develop_personaN` y una rama `feature/US-XX-...`.
- El tablero Kanban del equipo usa las columnas: **To Do → In Progress → In Review → Done**.

## Equipo

| Integrante | Repositorio personal |
|------------|----------------------|
| (completar) | `develop_persona1` |
| (completar) | `develop_persona2` |
| (completar) | `develop_persona3` |

## Definition of Done

- Los tres archivos del proyecto están presentes en `develop_central`.
- Existe la rama `develop` y contiene las contribuciones de todo el equipo.
- Cada integrante tiene su fork `develop_personaN` con al menos un PR mergeado.
- Issues, Milestone y tablero Kanban actualizados.

## Requisitos del entorno

- Navegador moderno (Chrome, Edge o Firefox actualizado).
- Conexion a internet la primera vez, para cargar Bootstrap y los iconos desde el CDN.
- Opcional: Python 3 o Node.js si prefieres servir la carpeta con un servidor local.
- Git 2.30+ y una cuenta de GitHub para participar en el flujo de ramas y Pull Requests.

## Como se generan las evidencias del laboratorio

| Paso | Evidencia |
|------|-----------|
| 5.1 | URL de `develop_central` + captura de la pagina Code con los archivos |
| 5.2 | Captura de la rama `develop` en el selector de ramas |
| 5.3 | Captura de Issues + Milestone + tablero Kanban |
| 5.4 | URL del fork `develop_personaN` + captura del repositorio |
| 5.5 | URL del PR + captura de *Files changed* y del PR mergeado |
| 5.6 | Historial de commits de `develop` y tablero completo en Done |
