# AutoKit

Aplicación web progresiva (PWA) en español para generar y organizar datos ficticios de prueba.

## Archivos
- `index.html`: aplicación completa.
- `manifest.webmanifest`: metadatos de instalación.
- `sw.js`: caché offline.
- `icon-192.png`, `icon-512.png`: iconos.

## Ejecutar
Para probar en computadora, sirve esta carpeta con cualquier servidor estático. Por ejemplo, con Python:
`python -m http.server 8000`
Abre `http://localhost:8000`. Para instalar en un iPhone se necesita publicar por HTTPS; `file://` no permite instalar una PWA ni activar el service worker.

## Publicación gratuita
1. Crea una cuenta gratuita en GitHub y un repositorio público llamado `autokit`.
2. Sube todos los archivos de esta carpeta a la raíz del repositorio.
3. En Settings → Pages, elige Deploy from a branch, selecciona `main` y `/ (root)`, y guarda.
4. Espera a que GitHub Pages publique el sitio HTTPS. La URL será similar a `https://TU-USUARIO.github.io/autokit/`.

## Instalar en iPhone
1. Abre la URL HTTPS en Safari.
2. Pulsa Compartir → Añadir a pantalla de inicio.
3. Activa “Abrir como app web” si aparece y pulsa Añadir.
4. Abre AutoKit desde el nuevo icono. Para actualizar, vuelve a abrir con conexión a internet.

## Privacidad y límites del navegador
Los registros y plantillas se guardan en `localStorage` del navegador y no se envían a un servidor. Borrar los datos del sitio o cambiar de navegador/dispositivo puede eliminarlos. Exporta un CSV si necesitas una copia.
Los teléfonos usan el bloque ficticio +1 202-555-0100 a 0199 y los correos usan dominios de ejemplo. No son datos de contacto reales.
Una PWA normal no puede leer ni modificar formularios de otras páginas: el aislamiento entre sitios lo impide. Usa copiar/pegar manualmente o integra APIs oficiales con autorización. AutoKit no evade CAPTCHA, autenticación, controles de acceso, límites ni programas de referidos.
