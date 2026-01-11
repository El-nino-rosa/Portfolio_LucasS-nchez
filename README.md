Página desplegada en Pages: https://el-nino-rosa.github.io/Portfolio_LucasS-nchez/
Este repositorio contiene mi portafolio web estático(diseñador gráfico e ilustrador). El proyecto está construido con HTML, CSS y JavaScript (vanilla) y organiza el contenido en páginas estáticas en la carpeta `secciones/` (Ilustración, Diseño, Motion). el porpósito de este proyecto es mostrar trabajos (ilustración, diseño y motion) en un layout ligero y accesible con una estética seria y moderna.
Modo de display "Gallery" con botones que abren un modal mostrando texto e imágenes/videos. 

Stack tecnológico:
- HTML5
- CSS3 (archivos en `assets/css/` y `assets/css/Secciones/`)
- JavaScript (vanilla) — `assets/js/main.js`
- Recursos estáticos: `assets/img/`, `assets/fonts/`, `assets/video/`

Desarrollo local:
1. Clona el repo o descarga el ZIP.
2. Abre PowerShell (Windows) o una terminal en la raíz del proyecto.
3. Ejecuta un servidor estático simple desde la raíz para evitar problemas de rutas relativas:

```powershell
python -m http.server 8000
```

4. Abre en el navegador:

http://localhost:8000/

Notas:
- El proyecto usa rutas relativas (p. ej. `../assets/...`) para las páginas dentro de `secciones/`. Servir desde un servidor local o desde GitHub Pages evita problemas de CORS y rutas.

Guía de personalización:
- Cambiar texto y títulos: edita los HTML en la raíz y en `secciones/`.
- Actualizar estilos globales: edita `assets/css/index.css`.
- Estilos por sección: `assets/css/Secciones/ilustracion.css`, `Diseño.css`, `Motion.css`.
- Añadir/editar proyectos en las secciones:
	- Cada proyecto en la galería está representado por un `<button class="gallery-item">` dentro de una `.gallery-grid`.
	- Propiedades útiles en cada `<button>`:
		- `data-title` — título que aparecerá en el modal.
		- `data-description` — descripción que aparece en el modal.
		- `data-images` — lista separada por comas con rutas relativas a imágenes o vídeos (mp4/webm/ogg). Ej: `data-images="../assets/img/foo.png, ../assets/video/clip.mp4"`.
		- `data-include-preview` — por defecto la imagen dentro del botón se incluye en la galería; establece `data-include-preview="false"` para excluirla.

- Modal y media:
	- El modal creará elementos `<img>` por defecto y `<video controls playsinline>` para entradas que terminen en `.mp4`, `.webm` o `.ogg`.
	- Puedes usar la imagen dentro del botón como `poster` añadiendo lógica en `assets/js/main.js` (se puede añadir si lo deseas).

Contacto

Para cambios rápidos sobre el contenido o subir assets, usa el repositorio. Para contacto directo: greattlucanopr@gmail.com

Uso de asistentes de IA:
Este proyecto ha contado con asistencia de herramientas de IA durante su desarrollo. A continuación se documenta de forma transparente cuándo y cómo se empleó la IA y el flujo obligatorio seguido para cualquier intervención asistida por IA.

Resumen de intervenciones asistidas por IA
- Correcciones de rutas y enlaces en páginas dentro de `secciones/`.
- Inserción y normalización de atributos `data-images` en botones de galería (`secciones/ilustracion.html`, `secciones/Diseño.html`, `secciones/Motion.html`).
- Implementación y mejoras en el modal de galería (`assets/js/main.js`) — ahora soporta imágenes y vídeos, opciones por botón para incluir/excluir la imagen previa, y manejo básico de accesibilidad (foco, Escape, tab-trap).
- Ajustes en estilos de sección (`assets/css/Secciones/ilustracion.css`) para mejorar la presentación del modal y las galerías.
- Creación y stylizado de la página `404.html`.

EL principal uso de IA en mi proyecto fue en el desarrollo de los gallery sections a través de Java Script, debido a que es un lenguaje que no se me hace tan comodo.

Fase obligatoria en dos pasos para cualquier uso de IA (POLÍTICA DEL PROYECTO)

Antes de integrar y aceptar los cambios propuestos por la IA (En mi caso, use en mayor proporción ChatGPT y también Copilot dentro de VSC), Localizé las lineas editadas y observe especificamente los cambios hechos y en que resultaban, analizando el razonamiento detrás de los cambios y comprendiendo el funcionamiento detrás de ellos.

Registro de cambios asistidos por IA:
Archivos modificados con asistencia: `secciones/ilustracion.html`, `secciones/Diseño.html`, `secciones/Motion.html`, `assets/js/main.js`, `assets/css/Secciones/ilustracion.css`, `404.html`

