# 🌐 WebGL Hub: Simulaciones Interactivas 3D con Three.js

Una aplicación web de portafolio que integra cinco simulaciones 3D interactivas renderizadas en tiempo real utilizando **Three.js** y **WebGL**. La interfaz principal está diseñada con un tema moderno estilo *Cyber-Tech / Neon Volt*, utilizando **Bootstrap 5** y efectos *Glassmorphism*.

## 🚀 Características Principales

*   **Menú Centralizado (Hub):** Un archivo `index.html` que carga las diferentes demostraciones mediante `iframes` de manera dinámica y responsiva.
*   **Diseño Moderno:** Interfaz de usuario (UI) personalizada con modo oscuro, tipografía técnica, efectos de resplandor neón (cyan/magenta/volt) y cuadrícula de fondo.
*   **Modularidad JS:** Cada demostración tiene su propio archivo HTML y su lógica aislada en archivos JavaScript independientes dentro de la carpeta `assets/js/`.
*   **Simulaciones Personalizadas:** Los parámetros base de Three.js fueron modificados (colores, geometrías, velocidades) para brindar una experiencia única en cada demo.

## 📂 Estructura del Proyecto

El proyecto sigue una arquitectura modular organizada de la siguiente manera:
```text
threejs-3d-models-5/
├── assets/
│   ├── build/              # Archivos core de Three.js (three.module.js)
│   ├── css/                # Hojas de estilo (Tema Neon Volt / Cyber-Tech)
│   ├── img/                # Recursos de imagen generales
│   ├── js/                 # Lógica principal de cada simulación
│   │   ├── main.js
│   │   ├── map.js
│   │   ├── minecraft.js    # Incluye lógica de colisión con el suelo
│   │   ├── orbit.js
│   │   ├── pointerlock.js
│   │   └── transform.js
│   ├── jsm/                # Addons de Three.js (controles, loaders, matemáticas)
│   │   ├── controls/
│   │   ├── curves/
│   │   ├── libs/
│   │   ├── loaders/
│   │   ├── math/
│   │   └── utils/
│   └── models/             # Modelos 3D adicionales 
├── index.html              # Menú principal (Hub de la aplicación)
├── map.html                # Demo 2: Map Controls
├── minecraft.html          # Demo 1: Generación procedural tipo Minecraft
├── orbit.html              # Demo 3: Orbit Controls con geometrías
├── pointerlock.html        # Demo 4: Controles de Primera Persona (FPS)
├── README.md               # Documentación del proyecto
└── transform.html          # Demo 5: Transform Controls (Mover, Rotar, Escalar)
```
## 🎮 Demostraciones Incluidas
* **Minecraft Geometry:** Generación de un terreno voxel procedural utilizando ruido de Perlin. Se le implementó un algoritmo de detección de altura en el eje Y para generar colisión con el suelo y evitar que la cámara atraviese el mapa.
* **Map Controls:** Demostración de controles de mapa interactivos, ideales para visualizar terrenos o ciudades desde una perspectiva isométrica/cenital.
* **Orbit Controls:** Visualización de múltiples figuras instanciadas en el espacio, permitiendo orbitar la cámara alrededor de un objetivo central.
* **PointerLock (FPS):** Simulación de controles de videojuego en primera persona. Usa captura del puntero del ratón, detección de colisiones con el entorno y físicas de gravedad para el salto.
* **Transform Controls:** Herramienta interactiva que permite manipular un objeto en el espacio 3D (traslación, rotación y escala) en tiempo real mediante gizmos visuales.

## 🛠️ Tecnologías Utilizadas
* **HTML5 & CSS3:** Estructuración y diseño visual (Grid, Flexbox, Variables CSS, Backdrop-filter).
* **JavaScript (ES6 Modules):** Lógica orientada a módulos (`import`/`export`) para mantener el código limpio.
* **Three.js (r128+):** Biblioteca de JavaScript para crear y mostrar gráficos 3D animados en un navegador web.
* **Bootstrap 5:** Framework de CSS para el sistema de cuadrículas (grid) y componentes responsivos del menú principal.

## 💻 Instalación y Uso
Para ejecutar este proyecto correctamente y evitar problemas de políticas de seguridad (CORS) al cargar módulos JS o texturas, es necesario montarlo sobre un servidor local.

1. Clona o descarga este repositorio.
2. Abre la carpeta del proyecto en tu editor de código (ej. Visual Studio Code).
3. Inicia un servidor local. Puedes usar la extensión **Live Server** en VS Code.
4. Abre `index.html` en tu navegador web.

## Programador

Desarrollado por: Antonio Yáñez Hernández.
Materia: Graficacion
Estudiante de Ingeniería en Sistemas Computacionales | Tecnológico Nacional de México