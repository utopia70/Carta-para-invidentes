# Mirador de la Isla · Carta accesible por voz

Página web estática para convertir la carta del restaurante **Mirador de la Isla** en una experiencia accesible mediante:

- Lectores de pantalla como VoiceOver y TalkBack.
- Navegación mediante teclado.
- Síntesis de voz para escuchar la carta.
- Reconocimiento de voz, cuando el navegador lo permite.

## Archivos

El proyecto necesita únicamente:

- `index.html` — página, estilos, carta, síntesis de voz y reconocimiento de voz.
- `README.md` — documentación del proyecto.

No necesita servidor, base de datos ni sistema de gestión de contenidos.

## Carta incluida

La primera versión contiene estas secciones:

1. Pescado frito
2. Pescado a la plancha
3. Carnes a la brasa

Los nombres y precios proceden de la transcripción incluida en la guía original y deben comprobarse contra la carta real antes de la publicación definitiva.

## Control por voz

Las órdenes previstas son:

- “carta completa”
- “pescado frito”
- “pescado a la plancha”
- “carnes a la brasa”
- “repetir opciones”
- “ayuda”
- “parar”

El navegador debe solicitar permiso para utilizar el micrófono. El reconocimiento de voz depende del dispositivo, navegador, sistema operativo y permisos disponibles.

Los botones de la página siguen funcionando aunque el reconocimiento de voz no esté disponible.

## Publicación con GitHub Pages

1. Crear un repositorio en GitHub, por ejemplo `carta-accesible`.
2. Subir `index.html` y `README.md` al nivel superior del repositorio.
3. Hacer `Commit changes`.
4. Entrar en **Settings → Pages**.
5. En **Build and deployment**, seleccionar **Deploy from a branch**.
6. Elegir la rama `main` y la carpeta `/(root)`.
7. Guardar.
8. Esperar a que GitHub publique el sitio.
9. Utilizar la dirección que proporciona GitHub Pages.

La dirección tendrá normalmente una forma similar a:

`https://USUARIO.github.io/carta-accesible/`

## Código QR

El QR debe apuntar a la página web publicada, no a un archivo de audio.

Conviene generar el QR definitivo únicamente después de comprobar la URL y probar la página en dispositivos reales.

Para facilitar su localización por una persona ciega, el QR debería acompañarse de una indicación táctil o en Braille y colocarse siempre en un lugar predecible.

## Pruebas recomendadas

Antes de publicar:

- Probar la página con VoiceOver en iPhone/iPad.
- Probarla con TalkBack en Android.
- Comprobar que todos los botones reciben el foco correctamente.
- Probar la activación del micrófono.
- Probar todas las órdenes de voz.
- Hacer una prueba completa sin mirar la pantalla.
- Comprobar la pronunciación de los nombres de los platos.
- Verificar todos los precios contra la carta original.
- Comprobar que las futuras modificaciones mantienen la misma URL.

## Mantenimiento

Para cambiar un precio o añadir/eliminar un plato, basta con modificar `index.html` y volver a confirmar los cambios en GitHub.

Mientras se mantenga la misma URL de GitHub Pages, el QR ya impreso seguirá funcionando.

## Referencias

- GitHub Docs — GitHub Pages.
- Guía original del proyecto: `Guia_carta_accesible_Mirador_de_la_Isla.docx`.
