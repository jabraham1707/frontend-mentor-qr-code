# Síntesis: Fundamentos de Maquetación Web
**Proyecto:** Componente de Código QR (Frontend Mentor)

## 1. Estructura y Semántica (HTML5)
El HTML no es solo para poner texto en pantalla; sirve para darle significado y contexto a la información, tanto para los navegadores como para los usuarios.

* **HTML Semántico (`<main>` vs `<div>`):**
  * `<div>` es un contenedor genérico sin significado, usado principalmente para agrupar elementos y aplicarles estilos CSS.
  * `<main>` indica cuál es el contenido principal y único de la página. Usarlo mejora la **accesibilidad** (lectores de pantalla) y el **SEO** (optimización para buscadores).
* **Diseño Responsivo (Etiqueta Viewport):**
  * `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  * Es la línea obligatoria para que la página no se vea diminuta en celulares. Le indica al navegador del dispositivo móvil que asuma su ancho real y no intente alejar el zoom como si fuera un monitor de escritorio.
* **Favicon:**
  * `<link rel="icon" type="image/png" ...>`
  * Sirve para enlazar el icono pequeño que aparece en la pestaña del navegador, dándole un acabado profesional al sitio.

## 2. Maquetación y Diseño (CSS3)
El control del diseño visual y la adaptación a diferentes tamaños de pantalla.

* **Centrado Perfecto con Flexbox:**
  * Se aplicó `display: flex;` al `body` junto con `justify-content: center;` (eje horizontal) y `align-items: center;` (eje vertical) y una altura de `min-height: 100vh;` para lograr que la tarjeta quede exactamente en el centro de la pantalla, sin importar su tamaño.
* **Imágenes Responsivas:**
  * En lugar de usar un ancho fijo en píxeles, asignar `max-width: 100%;` y `display: block;` a una imagen garantiza que esta se adapte al tamaño de su contenedor padre (`div`) sin desbordarse ni deformarse.
* **Posicionamiento Absoluto:**
  * `position: absolute;` saca a un elemento (como el pie de página de atribución) del flujo normal del documento, ignorando las reglas de Flexbox del contenedor padre. Combinado con `bottom: 15px;`, permite anclar el elemento en la parte inferior de la pantalla sin arruinar el centrado de la tarjeta principal.

## 3. Flujo de Trabajo Profesional (Git, GitHub y Despliegue)
Las herramientas estándar de la industria para gestionar el código y publicarlo.

* **Control de Versiones (Git Local):**
  * `git init`: Inicializa un nuevo repositorio en tu computadora.
  * `git add .`: Prepara todos los archivos modificados (Stage).
  * `git commit -m "mensaje"`: Crea un punto de guardado atómico y descriptivo.
  * `git branch -M main`: Renombra la rama principal al estándar actual de la industria.
* **Repositorio Remoto y Despliegue (GitHub):**
  * `git remote add origin <url>`: Conecta el código local con el servidor en la nube.
  * `git push -u origin main`: Sube los cambios de tu computadora a GitHub.
  * **GitHub Pages:** Una herramienta gratuita integrada en GitHub que toma los archivos estáticos de la rama `main` y los convierte en un sitio web en vivo con una URL pública.
