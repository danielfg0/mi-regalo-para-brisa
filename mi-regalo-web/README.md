# Mi regalo web ♡

Plantilla estática en HTML, CSS y JavaScript para crear una carta romántica interactiva, adaptable a celulares Android y iPhone, y publicarla gratis en GitHub Pages.

## Probarla en tu computadora

1. Descarga o descomprime la carpeta.
2. Abre `index.html` en Chrome, Firefox, Edge o Safari.
3. Personaliza los datos en el objeto `CONFIG`, al final de `index.html`.

## Personalizar

Busca `const CONFIG = {` al final del archivo. Cambia:

- `name1` y `name2`: nombres del encabezado.
- `heroSubtitle`: texto de portada.
- `letterGreeting`, `letterText` y `signature`: carta.
- `startDate`: fecha inicial en formato `AAAA-MM-DD`.
- `musicFile`: déjalo vacío o escribe, por ejemplo, `musica/cancion.mp3`.

Para fotos, agrega tres archivos llamados `foto-1.jpg`, `foto-2.jpg` y `foto-3.jpg` dentro de `fotos/`. Si tus archivos son PNG o WEBP, cambia las extensiones en los `src` correspondientes dentro de `index.html`.

Para música, agrega `cancion.mp3` dentro de `musica/`, cambia `musicFile` a `musica/cancion.mp3` y asegúrate de tener derecho a usar el audio. Los navegadores normalmente exigen que la persona toque el botón para comenzar la reproducción.

## Publicar gratis con GitHub Pages

1. Entra a https://github.com/ e inicia sesión o crea una cuenta.
2. Pulsa **New repository** (nuevo repositorio).
3. Ponle un nombre, por ejemplo `mi-regalo`, elige **Public** y crea el repositorio.
4. En el repositorio, pulsa **Add file → Upload files**.
5. Sube `index.html` y, si quieres, las carpetas `fotos/` y `musica/` con sus archivos. También puedes descomprimir la carpeta en tu computadora y arrastrar su contenido al área de carga. Asegúrate de que `index.html` quede en la raíz del repositorio.
6. Pulsa **Commit changes** para guardar.
7. En el repositorio, abre **Settings → Pages**.
8. En **Build and deployment**, elige **Deploy from a branch**. Selecciona la rama `main` y la carpeta `/(root)`, después pulsa **Save**.
9. Espera a que GitHub publique el sitio. La URL será parecida a `https://TU-USUARIO.github.io/mi-regalo/`. Puedes verla en Settings → Pages.
10. Abre ese enlace en tu teléfono y compártelo por WhatsApp.

## Qué incluye

- Diseño responsive para móvil, tablet y escritorio.
- Portada con nombres.
- Sobre/carta interactiva.
- Galería con espacios para tus fotos.
- Línea del tiempo editable.
- Contador de días.
- Vales interactivos.
- Botón de música opcional.

## Límites de esta versión

Esta es una página estática. Los vales guardan el estado solo en el navegador y dispositivo que los canjea; no se sincronizan entre teléfonos. No incluye cuentas, base de datos, editor para clientes ni pagos. GitHub Pages puede alojar el sitio estático sin costo, sujeto a las condiciones y límites de GitHub Pages.
