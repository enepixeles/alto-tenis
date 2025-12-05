# Proyecto: Landing Page "Alto Tenis"

Este proyecto consiste en el diseño y desarrollo de una Landing Page moderna para una escuela de tenis. El objetivo principal fue crear una interfaz de alto impacto visual, completamente responsiva y organizada bajo estándares profesionales de desarrollo Front-End.

## 📋 Planificación y Estructura del Proyecto

Para la construcción de este sitio, se planificó una arquitectura modular que separa la estructura (HTML), el estilo (SASS) y la lógica/interactividad (Bootstrap/jQuery).

### Organización de Archivos (Arquitectura 7-1)
Se utilizó el patrón arquitectónico 7-1 de SASS para mantener el código escalable y ordenado. La estructura de carpetas implementada es la siguiente:

*   **index.html**: Estructura semántica del sitio.
*   **css/**: Contiene el archivo compilado `main.css`.
*   **img/**: Recursos gráficos.
*   **scss/**: Código fuente de los estilos.
    *   **abstracts/**: Configuración global (Variables de color, fuentes, mixins).
    *   **base/**: Estilos base y resets (Tipografía general).
    *   **components/**: Módulos reutilizables (Botones, tarjetas).
    *   **layout/**: Estructura mayor (Header, Footer).
    *   **pages/**: Estilos específicos de cada vista (Home, secciones internas).
    *   **main.scss**: Archivo principal que importa y unifica todos los parciales.

---

## 🛠 Tecnologías y Herramientas Seleccionadas

### 1. Preprocesador: SASS (Syntactically Awesome Style Sheets)
**Elección:** Se eligió SASS (sintaxis .scss) como herramienta principal de estilo.

**Fundamentación (¿Por qué SASS?):**
*   **Organización Modular:** Permite dividir el CSS en pequeños archivos parciales (`_variables.scss`, `_home.scss`), facilitando la lectura y mantenimiento, a diferencia de tener un archivo CSS gigante de 1000 líneas.
*   **Uso de Variables:** Definimos una paleta de colores (`$color-cream`, `$color-black`) y fuentes centralizadas. Si la marca cambia de color, solo se edita una línea.
*   **Anidación (Nesting):** Permite escribir los selectores CSS siguiendo la jerarquía visual del HTML, lo que reduce la repetición de código y hace perfecta sinergia con la metodología BEM.

### 2. Metodología de Estilos: BEM (Block, Element, Modifier)
**Elección:** Se implementó la metodología de nomenclatura BEM.

**Fundamentación (¿Por qué BEM?):**
*   **Evita Conflictos:** Al usar nombres específicos como `.hero__title` o `.contact-section__input`, evitamos que un estilo afecte accidentalmente a otros elementos de la página (especificidad baja y controlada).
*   **Componentización:** Nos permite pensar en la interfaz como bloques independientes (Bloque "Hero", Bloque "Strength") que pueden moverse de lugar sin romperse.
*   **Claridad:** Cualquier desarrollador que lea el código HTML sabe qué relación tiene cada etiqueta con su contenedor padre.

### 3. Frameworks y Librerías
*   **Bootstrap 5:** Utilizado para el sistema de rejilla (Grid System), contenedores responsivos y componentes de navegación (Navbar). Permite agilizar la maquetación adaptable a móviles.
*   **jQuery:** Integrado para manipulación del DOM y soporte de funcionalidades dinámicas requeridas por el proyecto.

---

## 🎨 Decisiones de Diseño

*   **Tipografía:**
    *   *Títulos:* **Anton** (Google Fonts). Se eligió por su peso y estilo condensado para generar impacto y una sensación de fuerza/deporte.
    *   *Cuerpos de texto:* **Roboto**. Aporta legibilidad y modernidad.
*   **Paleta de Colores:**
    *   Negro / Dark Overlay: Elegancia y contraste.
    *   Crema (#f4f1ea) y Gris Claro (#F2F2F2): Para separar secciones de información de manera suave.

## 🚀 Instrucciones de Ejecución

1.  Asegurarse de tener la extensión **"Live Sass Compiler"** instalada en Visual Studio Code.
2.  Presionar "Watch Sass" en la barra inferior para compilar los estilos.
3.  Abrir el archivo `index.html` con "Live Server" o directamente en el navegador.

---
**Desarrollado para el curso: Desarrollo de Aplicaciones Front-End Trainee V2.0**