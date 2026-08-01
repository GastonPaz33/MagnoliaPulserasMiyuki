# Magnolia - Pulseras Miyuki

Sitio estático preparado para GitHub Pages, con catálogo editable y publicación de cambios mediante la API de GitHub. No usa Firebase.

## Archivos

- `index.html`: tienda + panel de administración oculto.
- `data.json`: productos, colores, banners y configuración pública.
- `assets/products/`: imágenes de productos.

## Publicar por primera vez

1. Creá un repositorio público en GitHub, por ejemplo `magnolia-tienda`.
2. Subí `index.html`, `data.json`, `README.md`, `.nojekyll` y la carpeta `assets/`.
3. Activá GitHub Pages desde `Settings > Pages`, usando `main` y `/ (root)`.

## Panel oculto

En la tienda, hacé 5 clics rápidos sobre el logo MAGNOLIA.

Usuario actual: `magnolia`

Contraseña actual: `magnolia2025`

Estas credenciales están dentro del JavaScript y no son seguridad real. Para un sistema profesional habría que reemplazar el acceso por una autenticación adecuada.

## Publicar productos e imágenes desde el panel

1. En GitHub creá un Fine-grained Personal Access Token.
2. Limitá el token al repositorio de Magnolia.
3. Dale permiso `Contents: Read and write`.
4. En el panel de administración, abrí `Configuración`.
5. Completá usuario, repositorio, rama y token.
6. Probá la conexión.
7. Editá o agregá productos.
8. Subí la foto desde el editor del producto.
9. Pulsá `🚀 Publicar cambios`.

El panel sube las imágenes a `assets/products/` y actualiza `data.json`. GitHub Pages vuelve a publicar el sitio después del commit.

Nunca pegues el token dentro de `index.html` ni lo compartas. El sistema solo lo mantiene en `sessionStorage` durante la sesión del navegador.
