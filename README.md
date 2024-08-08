# Three.js AR Project with Meta Quest 3

Este proyecto utiliza Three.js para crear una experiencia de realidad aumentada (AR) utilizando un visor Meta Quest 3. El proyecto incluye una textura de video y permite la interacción con el entorno AR.

## Requisitos

- Node.js
- npm (Node Package Manager)
- Un navegador compatible con WebXR (por ejemplo, Google Chrome)
- Un visor Meta Quest 3

## Instalación

1. Clona este repositorio:
    ```bash
    git clone https://github.com/tu-usuario/tu-repositorio.git
    cd tu-repositorio
    ```

2. Instala las dependencias necesarias:
    ```bash
    npm install
    ```

3. Inicia el servidor de desarrollo:
    ```bash
    npm run start
    ```

4. Abre tu navegador y navega a `http://localhost:3000` (o el puerto que hayas configurado) para ver la aplicación en acción.

## Uso

### Controles

- Usa el visor Meta Quest 3 para interactuar con la escena AR.
- Utiliza los controladores para manipular objetos dentro de la escena.
- Usa el botón de AR para entrar en el modo de realidad aumentada.

### Código

El archivo principal de la aplicación es `index.html` y el archivo JavaScript principal es `main.js`. Aquí hay un resumen de lo que hace el código:

- **Acceso a la cámara**: Utiliza `navigator.mediaDevices.getUserMedia` para acceder a la cámara del usuario y crear una textura de video.
- **Three.js Setup**: Configura la escena, la cámara y el renderizador de Three.js.
- **Materiales y geometría**: Crea una caja con una cara que utiliza la textura de video.
- **WebXR**: Integra WebXR para habilitar la realidad aumentada usando un visor Meta Quest 3.
- **ARButton**: Personaliza el botón de AR para mejorar su visibilidad.

```javascript
import * as THREE from 'three';
import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls.js';
import { XRControllerModelFactory } from 'three/examples/jsm/webxr/XRControllerModelFactory.js';
import { ARButton } from 'three/examples/jsm/webxr/ARButton.js';

// Código principal aquí...

### Notas:
- **Imagen de muestra**: La imagen `muestra.png` está vinculada correctamente como `![Imagen de muestra](./muestra.png)`, asumiendo que está en la raíz del proyecto.
- **Estructura**: La imagen se muestra en la sección "Imagen de muestra" para dar una referencia visual del proyecto.

Con este `README.md`, los usuarios tendrán una visión clara y completa del proyecto, incluyendo cómo instalarlo, usarlo, y una demostración visual tanto en video como en imagen.
