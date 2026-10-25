# NextMoment · web para GitHub Pages

Sitio estático para presentar la propuesta NextMoment de TecnoChallenge, conservar el prototipo interactivo y documentar la evolución del proyecto. Solo usa HTML, CSS y JavaScript; no necesita compilación, servidor backend ni dependencias de ejecución. Las imágenes, ilustraciones, logos, QR y vídeos están dentro de esta carpeta. El enlace a la aplicación publicada es externo de forma intencionada.

## Estructura

- `index.html`: portada, propuesta, perfiles del equipo, modelo de negocio, código QR y vídeo de demostración.
- `nuestra-causa.html`: valores, ODS y timeline de las diez ideas, primeros prototipos, mapas de empatía, EcoCanvas y aplicación final.
- `css/styles.css`, `js/main.js`: estilos responsive, navegación, animaciones y lightbox.
- `app/`: prototipo interactivo de la aplicación, con imágenes vectoriales locales de muestra.
- `assets/imagenes/`: recursos de marca, imágenes del equipo y del proceso, logos de Imaxel y TecnoCampus y QR.
- `assets/imagenes/equipo/`: fotografía grupal y retratos individuales de Carla, Hind (foto actualizada), Haotian, Eric y Gerard.
- `assets/videos/`: explicación del proyecto y demostración de la aplicación.
- `.nojekyll`: solicita a GitHub Pages servir también archivos y carpetas cuyo nombre comience con punto o guion bajo.

La identidad visual conserva el logotipo NextMoment y las variables CSS de la paleta original. Los logos de Imaxel y TecnoCampus aparecen con una indicación de contexto académico y empresarial, sin afirmar patrocinio ni certificación.

## Ejecutar localmente

Abre una terminal dentro de esta carpeta y ejecuta:

```powershell
py -m http.server 8000
```

Visita `http://localhost:8000`. También puedes abrir `index.html`, aunque el servidor local representa mejor las rutas relativas y la reproducción de vídeo.

## Vídeos

- `assets/videos/videoexplicativo.mp4`: H.264/AAC, 1920×1080, 79,39 s, **18.456.894 bytes**.
- `assets/videos/grabaciondemo.mp4`: H.264/AAC, 754×1372, 20,1 s, **7.895.782 bytes**.

El vídeo explicativo original HEVC/H.265 (93.456.016 bytes) sigue intacto en la raíz de TecnoChallenge, fuera de esta copia de publicación. La variante H.264/AAC conserva 1920×1080 y queda por debajo de 20 MB para ofrecer margen adicional. Ambos vídeos están por debajo del límite de 25 MB por archivo del cargador web de GitHub, así que puedes subir esta carpeta desde el navegador.

## QR y aplicación

`assets/imagenes/qr-nextmoment.png` es una imagen local de alto contraste. Codifica `https://hxial26.github.io/next-moment-app/`, igual que el botón «Probar NextMoment». El sitio no consulta un servicio de QR en tiempo de ejecución.

## Actualizar el contenido

- Edita `index.html` o `nuestra-causa.html` y conserva los enlaces relativos.
- Añade imágenes a `assets/imagenes/` y usa rutas como `assets/imagenes/proceso/nombre.png`.
- Sustituye vídeos manteniendo los nombres actuales o actualiza el `<source>` correspondiente. Se recomiendan MP4 H.264/AAC, sin `autoplay` y con `preload="metadata"`.
- Para cambiar el destino del QR, genera una nueva imagen PNG de alta resolución con la URL actualizada y reemplaza `assets/imagenes/qr-nextmoment.png`; actualiza también los dos botones externos.
- La app de ejemplo está en `app/`. Sus ilustraciones conceptuales locales no son fotografías de usuarios ni capturas del producto final.

Los mapas de empatía corresponden a una versión de investigación con 101 respuestas; el PDF inicial de ideas documenta una versión anterior con 83. La página identifica ambas bases y no mezcla sus porcentajes. Las ODS se presentan como relaciones temáticas, no como acreditaciones ni impactos demostrados.

## Publicar con GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube **el contenido de `NextMoment-GitHub` a la raíz del repositorio**, no la carpeta contenedora. Todos los archivos están por debajo de 25 MB y se pueden añadir desde el navegador.
3. Abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**.
5. Elige la rama `main` y la carpeta `/ (root)`.
6. Guarda y espera a que GitHub termine el despliegue.
7. Visita la dirección pública que aparecerá en Settings → Pages, normalmente `https://usuario.github.io/nombre-repositorio/`.

Las referencias locales son relativas para que funcionen bajo la ruta del repositorio, no solo en la raíz del dominio.
