# Guía para publicar la web del Círculo en GitHub Pages

Esta guía está pensada para hacerlo todo desde el navegador, sin instalar nada y sin línea de comandos. Sigue los pasos en orden la primera vez; a partir de ahí, actualizar la web será muy rápido.

## Antes de empezar

Ten a mano, en una carpeta de tu ordenador, todos los archivos de la web, respetando esta estructura de carpetas tal cual:

- index.html
- que-es.html
- actividades.html
- espiritualidad.html
- editor.html
- La carpeta assets, y dentro de ella:
  - datos.json
  - estilo.css
  - La carpeta img con los tres logos (logo-circulo.png, logo-movement.png, logo-arrupe.png)

La estructura importa: si un archivo acaba en el sitio equivocado, la web se ve sin estilo. Respeta las carpetas tal como están.

## Paso 1 · Crear la cuenta y el repositorio

1. Entra en github.com e inicia sesión (o crea una cuenta gratuita si aún no la tienes).
2. Arriba a la derecha, pulsa el signo "+" y elige "New repository".
3. En "Repository name" escribe un nombre sencillo, por ejemplo laudatosivlc.
4. Déjalo como "Public". GitHub Pages gratuito necesita que el repositorio sea público.
5. No marques ninguna casilla de añadir README ni nada más.
6. Pulsa "Create repository".

Quedará una página que dice, entre otras cosas, "uploading an existing file". Ese es el enlace que usaremos para subir la web.

## Paso 2 · Subir los archivos

1. En esa página del repositorio recién creado, busca el enlace "uploading an existing file" y púlsalo. Si ya no lo ves, ve a la pestaña "Add file" (arriba) y elige "Upload files".
2. Abre la carpeta de tu ordenador donde tienes la web.
3. Arrastra a la ventana del navegador los cinco archivos .html y la carpeta assets entera de una vez. GitHub respeta las carpetas al arrastrarlas, así que assets subirá con todo su contenido dentro.
4. Espera a que aparezcan todos en la lista. Comprueba que ves assets/estilo.css, assets/datos.json y assets/img/ con los logos: eso confirma que las carpetas se subieron bien.
5. Baja hasta el recuadro "Commit changes" y pulsa el botón verde "Commit changes". "Commit" significa simplemente confirmar y guardar los cambios.

Si arrastrar la carpeta no te funcionara, puedes subir los archivos sueltos y luego crear la carpeta escribiendo assets/estilo.css como nombre al subir cada archivo; pero lo normal es que arrastrar la carpeta funcione a la primera.

## Paso 3 · Activar GitHub Pages

1. En tu repositorio, entra en la pestaña "Settings" (arriba del todo).
2. En el menú de la izquierda, pulsa "Pages".
3. En "Source", elige "Deploy from a branch".
4. En "Branch", selecciona "main" y, en la carpeta, deja "/ (root)". Pulsa "Save".
5. Espera uno o dos minutos y recarga la página. Aparecerá arriba un recuadro con la dirección de tu web, del estilo https://tuusuario.github.io/laudatosivlc/

Esa es la dirección pública de la web del Círculo. Ábrela para comprobar que se ve bien. La primera vez puede tardar un par de minutos en estar disponible.

## Paso 4 · Comprobar que todo funciona

Abre la dirección de tu web y verifica:

- La portada se ve con su diseño, colores y el logo del Círculo arriba.
- El menú (icono de tres rayas en móvil) abre y los enlaces llevan a Actividades, Espiritualidad y Qué es el Círculo.
- Las páginas cargan su contenido.

Si la web se viera sin estilo, como una lista de texto plano, casi seguro es que la carpeta assets no quedó en su sitio. Vuelve al repositorio, comprueba que existe la carpeta assets con estilo.css dentro, y si no, vuelve a subirla respetando la estructura.

## Cómo actualizar la web más adelante

Cada vez que quieras cambiar textos, citas, fotos o la zona de miembros, el flujo es este:

1. Abre editor.html en tu ordenador y haz los cambios.
2. Pulsa "Guardar y descargar". Se te descargará datos.json y, si cambiaste fotos, también las imágenes.
3. Ve a tu repositorio en github.com.
4. Para reemplazar datos.json: entra en la carpeta assets, pulsa sobre datos.json, pulsa el icono del lápiz (o "Add file" y "Upload files" para sustituirlo), sube el nuevo y confirma con "Commit changes". Al subir un archivo con el mismo nombre y en la misma carpeta, GitHub lo reemplaza.
5. Para las fotos: súbelas a la carpeta assets/img de la misma manera.
6. En uno o dos minutos, la web se actualiza sola.

Consejo práctico: la forma más cómoda de sustituir archivos es siempre "Add file" y luego "Upload files", arrastrando el archivo nuevo con el mismo nombre y en la misma carpeta. GitHub entiende que es una versión nueva y lo reemplaza al confirmar.

## Publicar la zona de miembros

1. En el editor, en el apartado "Zona de miembros", prepara el contenido, adjunta los PDF, pon la contraseña y pulsa "Generar miembros.html cifrado".
2. Sube el miembros.html descargado a la raíz del repositorio (junto a index.html), igual que los demás archivos.
3. El enlace "Zona de miembros" del menú ya apunta a esa página.

Recuerda: guarda la contraseña en un lugar seguro. Si se pierde, el contenido cifrado no se puede recuperar.

## Si algo va mal

- La web se ve sin diseño: la carpeta assets no está en su sitio. Revísala en el repositorio.
- Los logos no aparecen: comprueba que están en assets/img con exactamente esos nombres.
- Un cambio no se refleja: espera un par de minutos y recarga; GitHub Pages tarda un poco en actualizar.
- La dirección da error 404 al principio: es normal en los primeros minutos tras activar Pages; espera y recarga.
