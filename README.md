# One Social Run San Javier

Web estática mobile-first. No necesita Python, servidor ni instalación.

## Uso

Abre `index.html` con cualquier navegador moderno. Para publicarla en GitHub Pages, sube `index.html` y la carpeta `assets` a la raíz del repositorio, selecciona `main` y `/(root)` en Settings > Pages.

## Qué incluye

- Próxima quedada, cartel, detalles y confirmación local.
- Presentación de la filosofía del grupo.
- Galería con imágenes reales proporcionadas.
- Galería pública de solo lectura, actualizada directamente en los archivos de la web.
- Compartir mediante el menú nativo del móvil.
- Preguntas frecuentes e Instagram.
- Diseño específico para teléfono y adaptación a escritorio.

## Importante

La web utiliza Firebase Authentication y Firestore, sin Storage ni plan Blaze. Los visitantes pueden iniciar sesión con Google y gestionar su propia asistencia. El administrador `jesussoler2003@gmail.com` puede crear, editar, finalizar y eliminar quedadas; consultar asistentes; y administrar las rutas de imágenes de la galería.

Las fotografías se suben manualmente a `assets` en GitHub. Después el administrador añade la ruta desde el panel privado, por ejemplo `assets/quedada-agosto.jpg`.

## Activación imprescindible

1. En Firebase Authentication activa Google como proveedor.
2. En Firestore abre la pestaña Reglas, pega todo el contenido de `firestore.rules` y pulsa Publicar.
3. Sube todos estos archivos a la raíz de GitHub Pages.
4. Abre la web publicada, pulsa Entrar y usa `jesussoler2003@gmail.com`.
5. Aparecerá el botón Gestionar. Desde ahí crea la primera quedada.

Si Google muestra `auth/unauthorized-domain`, abre Authentication > Configuración > Dominios autorizados y añade tu dominio `USUARIO.github.io`.
