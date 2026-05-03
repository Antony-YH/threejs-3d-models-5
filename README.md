# Visor de Animaciones 3D con Three.js

Este proyecto consiste en una aplicación web interactiva desarrollada con **Three.js** que permite la visualización y control de modelos 3D animados en formato FBX. La implementación destaca por la integración de esqueletos animados (Skins) y el uso de herramientas de monitoreo de rendimiento y control de parámetros en tiempo real.

## 🚀 Características

- **Carga de Modelos FBX:** Uso de `FBXLoader` para importar modelos complejos con jerarquías de huesos y animaciones.
- **Control de Animación:** Integración de `AnimationMixer` para reproducir de forma fluida el clip de animación (Samba Dancing).
- **Cámara Interactiva:** Implementación de `OrbitControls` para permitir al usuario rotar, acercar y desplazar la cámara alrededor del personaje.
- **Interfaz de Usuario (GUI):** Uso de `lil-gui` para la manipulación dinámica de *Morph Targets* y otros parámetros del modelo.
- **Monitoreo de Rendimiento:** Inclusión de `Stats.js` para visualizar los FPS (cuadros por segundo) y latencia de renderizado.
- **Entorno Gráfico:** Configuración de iluminación hemisférica, niebla y sombras proyectadas.

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** JavaScript (ES6+).
* **Motor Gráfico:** [Three.js](https://threejs.org/) (WebGL).
* **Formato de Modelo:** FBX (vía Mixamo).
* **Bibliotecas Adicionales:**
    * `fflate`: Para la descompresión rápida de datos del modelo.
    * `lil-gui`: Panel de control interactivo.
    * `stats.js`: Medidor de rendimiento.

## 📂 Estructura del Proyecto

A partir de los archivos implementados, la estructura es la siguiente:

```text
/
├── index.html              # Punto de entrada y configuración de importmap
├── assets/
│   ├── css/
│   │   └── main.css        # Estilos visuales de la interfaz
│   ├── js/
│   │   └── main.js         # Lógica principal de la escena y el bucle de renderizado
│   ├── build/
│   │   └── three.module.js # Núcleo de la biblioteca Three.js
│   ├── jsm/                # Módulos y complementos (Addons)
│   │   ├── controls/
│   │   │   └── OrbitControls.js
│   │   ├── loaders/
│   │   │   └── FBXLoader.js
│   │   ├── libs/
│   │   │   ├── fflate.module.js
│   │   │   ├── stats.module.js
│   │   │   └── lil-gui.module.min.js
│   │   └── curves/         # Utilidades para curvas NURBS
│   │       ├── NURBSCurve.js
│   │       └── NURBSUtils.js
│   └── models/
│       └── fbx/
│           └── Samba Dancing.fbx # Modelo 3D y animación principal
```

## Programador

Desarrollado por: Antonio Yáñez Hernández.
Materia: Graficacion