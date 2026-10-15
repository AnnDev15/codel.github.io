# Reconstrucción responsive de CODEL

Archivos incluidos:

- `index.html`
- `styles.css`
- carpeta `assets/` para colocar imágenes y logotipos

## Cómo agregar imágenes

Puede sustituir cada bloque con clase `image-placeholder` por una etiqueta:

```html
<img src="assets/nombre-imagen.jpg" alt="Descripción de la imagen">
```

Para conservar la forma de una imagen principal:

```css
.hero-visual img {
  width: 100%;
  min-height: 590px;
  object-fit: cover;
  border-radius: 52% 48% 42% 58% / 42% 42% 58% 58%;
}
```

En las tarjetas de categorías:

```html
<article class="category-card">
  <img class="category-image" src="assets/cocinas.jpg" alt="Cocinas">
  ...
</article>
```

La clase `.category-image` ya tiene el tamaño necesario. Agregue:

```css
img.category-image {
  object-fit: cover;
}
```

## Observaciones

- El menú móvil funciona únicamente con HTML y CSS.
- Se incluyeron puntos de quiebre para escritorio, tablet y móvil.
- Los textos y bloques siguen la estructura visible del sitio analizado.
- Las cifras pueden ajustarse a los datos reales de CODEL.
- El botón de WhatsApp usa el número +505 7550 4754.
