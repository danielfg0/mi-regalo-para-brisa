# Regalo de cumpleaños para Brisa ♡

Una página web romántica estática hecha con HTML, CSS y JavaScript. No necesita frameworks, instalar paquetes, base de datos ni pagar alojamiento para una primera versión. Está diseñada para verse en Android, iPhone y computadora.

## Archivos y carpetas

```text
mi-regalo-brisa/
├── index.html
├── README.md
├── fotos/
│   ├── INSTRUCCIONES.txt
│   ├── foto-1.jpg       <- agrega tu foto aquí
│   ├── foto-2.jpg       <- agrega tu foto aquí
│   └── foto-3.jpg       <- agrega tu foto aquí
└── musica/
    ├── INSTRUCCIONES.txt
    └── cancion.mp3      <- agrega tu canción aquí
```

Los archivos `foto-1.jpg`, `foto-2.jpg`, `foto-3.jpg` y `cancion.mp3` son ejemplos de nombres que debes usar para tus propios archivos; no se incluyen fotos ni música con derechos de autor. Si todavía no agregas las fotos, la página muestra marcadores bonitos. El botón de música espera el archivo `musica/cancion.mp3`.

## Cómo personalizar

Abre `index.html` con Visual Studio Code, Bloc de notas u otro editor de texto. Busca `const CONFIG = {` casi al final del archivo. Cambia estos campos:

- `birthdayName`: nombre de tu novia.
- `fromName`: tu nombre.
- `heroSubtitle`: frase que aparece en la portada.
- `letterGreeting`: saludo de la carta.
- `letterText`: contenido de la carta. Puedes dejar líneas en blanco usando dos saltos `\n\n` dentro del texto.
- `signature`: firma que aparece al final de la carta (puedes personalizarla).
- `startDate`: fecha desde la que cuentan los días, en formato `AAAA-MM-DD`.
- `musicFile`: ruta al MP3. Para la carpeta incluida, déjalo como `musica/cancion.mp3`.

También puedes buscar en el HTML los comentarios `EDITA LOS RECUERDOS` para cambiar los pies de foto y los tres momentos de la historia. Los textos de los cupones se cambian buscando `data-coupon`.

## Cómo añadir fotos

1. Elige tres fotos y, si hace falta, recórtalas para que se vean bien en vertical.
2. Renómbralas exactamente `foto-1.jpg`, `foto-2.jpg` y `foto-3.jpg` (o cambia sus rutas en `index.html`).
3. Colócalas dentro de `fotos/`.
4. Si la foto es PNG, WebP u otro formato, cambia también la extensión en la etiqueta `<img src="...">` del HTML. GitHub distingue mayúsculas y minúsculas en los nombres.

## Cómo añadir la canción

1. Coloca el archivo MP3 dentro de `musica/`.
2. El nombre debe ser exactamente `cancion.mp3`.
3. En la configuración debe quedar `musicFile: "musica/cancion.mp3"`.
4. En celular, toca el botón «Reproducir canción»: los navegadores normalmente no permiten que la música arranque sola. Usa una canción que tengas derecho a compartir.

## Publicar gratis con GitHub Pages

### Método recomendado: subir todos los archivos juntos

1. Descomprime `mi-regalo-brisa.zip` en tu computadora.
2. Entra a tu repositorio de GitHub. Si ya tiene el `index.html` anterior, reemplázalo con el nuevo `index.html` al hacer la carga, o bórralo antes de subir el nuevo.
3. Pulsa **Add file → Upload files**.
4. Abre la carpeta descomprimida y arrastra al área de carga `index.html`, `README.md` y las carpetas `fotos` y `musica` con sus archivos. Comprueba en la lista previa que las rutas estén dentro de sus carpetas. Si el navegador no acepta arrastrar las carpetas, entra en cada carpeta y sube sus archivos en su ruta correspondiente; puedes crear la ruta con **Add file → Create new file** usando por ejemplo `fotos/INSTRUCCIONES.txt` y luego subir cada foto.
5. Pulsa **Commit changes** para guardar todo.
6. En el repositorio, abre **Settings → Pages**. En **Build and deployment**, selecciona **Deploy from a branch**, rama **main**, carpeta **/(root)** y guarda.
7. En la misma sección aparecerá el enlace público de tu página. Ábrelo en el celular y prueba carta, fotos y canción.

Si la página ya estaba publicada, conserva la configuración de Pages: al subir un cambio a `main`, GitHub vuelve a publicar automáticamente. Puede tardar unos minutos.

## Importante

- La página es estática y no tiene cuentas, editor en línea ni base de datos.
- Los cupones se guardan en el almacenamiento local del navegador de ese dispositivo; no se comparten entre teléfonos.
- Un repositorio público significa que el código y cualquier foto/canción que subas serán accesibles para otras personas. No subas nada privado.
- GitHub Pages sirve para una página estática personal. Si más adelante quieres convertirla en un negocio donde otras personas creen páginas y hagan pagos, necesitarás una arquitectura y alojamiento apropiados para eso.
