# HTML MASTER EDITOR — listo para publicar

## Archivos
- `index.html` — la app completa (editor + vista previa en vivo), autocontenida y sin dependencias externas.
- `sw.js` — Service Worker que habilita el uso sin conexión una vez instalada como PWA.

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub (o usa uno existente).
2. Sube `index.html` y `sw.js` a la raíz del repositorio (deben quedar en la misma carpeta).
3. Ve a **Settings → Pages**, elige la rama (`main`) y la carpeta raíz (`/`), y guarda.
4. Espera 1–2 minutos; GitHub te dará una URL tipo `https://tu-usuario.github.io/tu-repo/`.
5. Abre esa URL desde el celular o la computadora: el navegador ofrecerá **"Instalar app"** (con el ícono `</>`). Una vez instalada, funciona sin internet gracias a `sw.js`.

## Uso local (sin subir nada)
También puedes abrir `index.html` con doble clic directamente — funciona igual, solo que sin la opción de "instalar como app" (eso requiere HTTPS).
