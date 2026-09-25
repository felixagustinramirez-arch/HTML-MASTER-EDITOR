# HTML MASTER EDITOR — listo para publicar

## Archivos
- `index.html` — la app completa (editor + vista previa en vivo), autocontenida y sin dependencias externas.
- `sw.js` — Service Worker que habilita el uso sin conexión una vez instalada como PWA.

## Tu trabajo se guarda solo
Cada cambio se guarda automáticamente en el propio dispositivo (usando IndexedDB, similar a localStorage pero sin su límite de tamaño, clave para proyectos con imágenes). Si cierras la pestaña, se apaga el celular o pierdes internet, al volver a abrir la app tu proyecto sigue ahí tal como lo dejaste. El "· guardado" que aparece junto a LIVE confirma cada guardado.

Para borrar todo y empezar de cero, usa el botón "🗑 borrar todo" en la fila de archivos (pide confirmación antes de borrar).

## Carpetas e importación
- Para organizar tu proyecto en subcarpetas, al crear un archivo nuevo usa una ruta como `paginas/menu.html` o `css/theme.css` — la carpeta se crea sola.
- "⭱ importar" carga uno o varios archivos sueltos desde tu dispositivo.
- "📁 importar carpeta" carga una carpeta completa conservando su estructura (disponible en navegadores de escritorio/Android; en iPhone puede comportarse como selección múltiple normal).
- Los archivos `.html/.css/.js` se importan como código editable; todo lo demás (imágenes, PDFs, etc.) se importa como recurso, igual que "+ imagen/doc".

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub (o usa uno existente).
2. Sube `index.html` y `sw.js` a la raíz del repositorio (deben quedar en la misma carpeta).
3. Ve a **Settings → Pages**, elige la rama (`main`) y la carpeta raíz (`/`), y guarda.
4. Espera 1–2 minutos; GitHub te dará una URL tipo `https://tu-usuario.github.io/tu-repo/`.
5. Abre esa URL desde el celular o la computadora: el navegador ofrecerá **"Instalar app"** (con el ícono `</>`). Una vez instalada, funciona sin internet gracias a `sw.js`.

## Uso local (sin subir nada)
También puedes abrir `index.html` con doble clic directamente — funciona igual, solo que sin la opción de "instalar como app" (eso requiere HTTPS).

