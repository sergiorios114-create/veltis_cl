# Veltis Latam — Sitio Corporativo (v1)

Prototipo del home page para Veltis Latam, holding de servicios para la continuidad operacional de la gran minería.

## Requisitos

Ninguno. Es HTML/CSS/JS estático. Para verlo en local solo necesitas un servidor web simple.

## Correr local

```bash
# Con Python
python3 -m http.server 8000

# Con Node (si tienes npx)
npx serve .
```

Luego abrir `http://localhost:8000` en el navegador.

## Publicar en GitHub Pages

1. Sube el contenido de esta carpeta a tu repositorio.
2. En el repo: **Settings → Pages →** Source: `Deploy from a branch`, branch `main` (carpeta `/root`).
3. Espera el deploy y abre la URL que entrega GitHub.

> **IMPORTANTE — por qué se incluye `.nojekyll`:** GitHub Pages procesa el sitio con **Jekyll**, y Jekyll **ignora las carpetas que empiezan con guion bajo** (`_img`, `_video`). Sin el archivo `.nojekyll` en la raíz, las imágenes y los videos **no se publican** (aparecen rotos). El archivo `.nojekyll` (vacío) desactiva ese procesamiento y sirve las carpetas tal cual. **No lo borres.**

## Dependencias externas (CDN)

- [GSAP](https://gsap.com) + [ScrollTrigger](https://gsap.com/docs/v3/Plugins/ScrollTrigger/) — animaciones
- [Lenis](https://lenis.studiofreight.com) — smooth scroll
- Google Fonts: Manrope + Source Sans 3

> Requiere conexión a internet para cargar fuentes y librerías desde CDN.

## Estructura

```
.nojekyll           → desactiva Jekyll en GitHub Pages (necesario, ver arriba)
index.html          → Home page
_img/               → Imágenes (fotos de faena)
_img/logos/         → Logos de Veltis y marcas (Berliam, Steel, Walvis, Quintrax)
_video/             → Video hero (loop) + poster
README.md
```

## Notas

- Diseño: base blanco/negro + acento amarillo `#ffc72c` (uso racionado).
- Tipografía: Manrope (títulos) + Source Sans 3 (cuerpo).
- Contenido oficial verificado vs Google Doc (junio 2026).
- Las imágenes y videos son placeholders del banco de Veltis para mostrar al cliente.
