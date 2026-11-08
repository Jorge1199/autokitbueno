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
El generador crea nombres ficticios, usuarios con dos dígitos y direcciones @gmail.com candidatas no verificadas. Permite seleccionar 998 (Cancún), 786/305 (Miami), 641 (Iowa), 614 (Ohio), 212 (Nueva York), 213 (California), 312 (Illinois), 404 (Georgia), 702 (Nevada), 713 (Texas), 615 (Tennessee), 617 (Massachusetts), 206 (Washington) y 602 (Arizona). Los teléfonos son marcadores de prueba no operativos: para EE. UU. se usa el bloque ficticio 555-0100 a 555-0199; para México se ocultan los dígitos centrales. No crean cuentas ni líneas activas y no sirven para recibir SMS o verificar registros reales. No crea cuentas ni líneas activas. Para registros reales, utiliza una dirección Gmail creada por ti y un número asignado por tu operador.
Una PWA normal no puede leer ni modificar formularios de otras páginas: el aislamiento entre sitios lo impide. Usa copiar/pegar manualmente o integra APIs oficiales con autorización. AutoKit no evade CAPTCHA, autenticación, controles de acceso, límites ni programas de referidos.

## Datos personales locales
La sección **Mis datos** permite guardar nombre, correo y teléfono en el almacenamiento local del dispositivo y copiarlos manualmente. No se envían a páginas externas ni se rellenan o envían formularios automáticamente.
