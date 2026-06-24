# Veltis Latam — Sitio Corporativo (v1)

Prototipo del home page para Veltis Latam, holding de servicios para la continuidad operacional de la gran minería.

## Correr local

```bash
python3 -m http.server 8000   # o:  npx serve .
```
Abrir `http://localhost:8000`.

## Publicar en GitHub Pages

1. Sube esta carpeta a tu repositorio.
2. **Settings → Pages → Source: "Deploy from a branch"**, branch `main`, carpeta `/ (root)`.
3. Espera el deploy (~1 min) y abre la URL. Si no ves cambios, recarga con `Ctrl+Shift+R`.

> Las carpetas de assets se llaman `img/` y `video/` (sin guion bajo) a propósito: así GitHub Pages las publica sin necesidad de un archivo `.nojekyll`.

## Estructura

```
index.html      → Home page
img/            → Imágenes (fotos de faena)
img/logos/      → Logos de Veltis y marcas (Berliam, Steel, Walvis, Quintrax)
video/          → Video hero (loop) + poster
README.md
```

## Dependencias externas (CDN — requieren internet)

- GSAP + ScrollTrigger (animaciones) · Lenis (smooth scroll) · Google Fonts: Manrope + Source Sans 3

## Notas

- Diseño: base blanco/negro + acento amarillo `#ffc72c` (uso racionado).
- Tipografía: Manrope (títulos) + Source Sans 3 (cuerpo).
- Imágenes y video son placeholders del banco de Veltis para mostrar al cliente.
