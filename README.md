
# Sitio web — ArgenPuerto SRL

Sitio corporativo estático, listo para desplegar gratis (GitHub Pages / Netlify / Vercel).

## Estructura

- `index.html` — Inicio (servicios, clientes, CTA)
- `servicios.html` — Detalle de servicios
- `proyectos.html` — Proyectos de referencia
- `nosotros.html` — Propósito, valores y gestión
- `contacto.html` — Formulario (Netlify Forms) y datos de contacto
- `politica-privacidad.html` — Texto base de privacidad
- `assets/` — Estilos, scripts e imágenes (SVG)

## Paleta de colores (personalizada)

- Azul oscuro (`--primary`): #0B2B4C
- Naranja (`--accent`): #FF6A00
- Verde claro (`--secondary`): #2ECC71

Puede ajustar variables en `assets/css/style.css`.

## Despliegue rápido (gratuito)

### Opción A) Netlify (recomendada para el formulario)
1. Cree una cuenta en https://app.netlify.com e inicie sesión.
2. "Add new site" → **Deploy manually** y arrastre la carpeta del proyecto.
3. Abra **Forms** en Netlify y verifique que el formulario `contacto` esté detectado.
4. Configure notificaciones al email y reCAPTCHA si desea.

### Opción B) GitHub Pages
1. Cree un repositorio nuevo en GitHub y suba todos los archivos.
2. En *Settings* → *Pages*, seleccione la rama `main` y la carpeta raíz `/`.
3. Espere 1–2 minutos; su sitio quedará disponible en `https://usuario.github.io/REPO`.
4. **Importante:** El formulario no enviará datos en GitHub Pages (no hay backend). Use `mailto:` o servicios como Formspree.

### Opción C) Vercel
1. Suba el repositorio a GitHub.
2. Conecte el repo en https://vercel.com/new y despliegue.

## Personalización

- Reemplace emails, teléfonos y enlaces en `footer` y `contacto.html`.
- Actualice `application/ld+json` en los archivos HTML con su sitio real y dirección.
- Sustituya los logos de clientes en la sección *Clientes*.
- Si lo desea, agregue su favicon en PNG (32×32) y actualice el `<link rel="icon">`.

## Formulario sin Netlify

Edite `contacto.html` y cambie el `<form>` por:

```html
<form action="https://formspree.io/f/XXXXXXX" method="POST">
  ...campos...
</form>
```

Cree su endpoint gratuito en Formspree y reemplace `XXXXXXX`.

## SEO básico

- Meta descripción incluida.
- JSON-LD de `Organization` para buscadores.
- `sitemap.xml` y `robots.txt` incluidos.

## Licencia

Uso libre. Requiere reemplazar los datos de ejemplo por los de su empresa.
