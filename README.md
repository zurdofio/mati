# Sinergia Studio

Sitio web institucional de **Sinergia Studio** — Franco Matías Luna · Coaching, entrenamiento y desarrollo deportivo. Córdoba, Argentina.

Single-page, responsive, HTML/CSS/JS sin dependencias de build. Listo para GitHub Pages.

## Estructura

```
.
├── index.html                 # Toda la página (HTML + CSS + JS en un archivo)
├── .nojekyll                  # Evita el procesamiento Jekyll en GitHub Pages
└── assets/
    ├── sinergia-mark-white.png  # Isologo en blanco (fondos oscuros)
    ├── sinergia-mark-black.png  # Isologo en negro (fondos claros)
    ├── sinergia-logo.png        # Logo original (cuadro completo)
    ├── signature-black.png      # Firma manuscrita (fondos claros)
    ├── signature-white.png      # Firma manuscrita (fondos oscuros)
    └── favicon-32/64/180.png    # Favicons
```

## Publicar en GitHub Pages

1. Crear un repositorio en GitHub y subir estos archivos:
   ```bash
   git init
   git add .
   git commit -m "Sinergia Studio — sitio web"
   git branch -M main
   git remote add origin https://github.com/USUARIO/REPO.git
   git push -u origin main
   ```
2. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. El sitio queda disponible en `https://USUARIO.github.io/REPO/` en un par de minutos.

> Para un dominio propio, agregar un archivo `CNAME` con el dominio y configurarlo en **Settings → Pages**.

## Ver el sitio en tu computadora (opcional)

No necesita instalación: alcanza con abrir `index.html` en el navegador. Si preferís un servidor local:

```bash
python3 serve.py    # luego abrí http://127.0.0.1:4317
```

> Los archivos `serve.py` y la carpeta `.claude/` son solo ayudas para la vista previa local. Podés borrarlos antes de publicar; no afectan al sitio.

## Cómo editar el contenido

Todo el contenido y los estilos viven en `index.html`:

- **Textos**: editar directamente el HTML de cada sección (`Filosofía`, `Enfoque`, `Servicios`, `Trayectoria`, `Formación`, `Contacto`).
- **Colores y tipografías**: variables CSS en `:root` al inicio del `<style>`.
- **Contacto**: bloque `id="contacto"`.
  - **LinkedIn**: cuando el perfil esté creado, reemplazar el `<div class="ch soon" ...>` (marcado con el comentario *LinkedIn: reemplazar href...*) por un `<a class="ch" href="URL_DEL_PERFIL" target="_blank" rel="noopener">` y actualizar el texto.
  - **WhatsApp / Email / Instagram**: verificar que los enlaces correspondan a los datos definitivos.

## Datos a confirmar

- **WhatsApp**: `+54 9 351 207-9969` (enlace `https://wa.me/5493512079969`) — tomado del CV. Confirmar o reemplazar.
- **Email**: `francomatiasluna@gmail.com` — tomado del CV. Confirmar o reemplazar.
- **LinkedIn**: pendiente de creación (placeholder activo).
