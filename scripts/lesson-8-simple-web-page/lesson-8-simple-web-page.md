# Lección 8: Desarrollo de una página web sencilla

En esta lección reunirás HTML y CSS para crear una página sobre tus intereses. Trabajarás con un ejemplo llamado **Mi espacio creativo**: una tarjeta con un título, una presentación, una lista de pasatiempos, dos imágenes, un enlace y un campo para escribir.

HTML organiza el contenido y CSS define su apariencia. No necesitas memorizar las etiquetas: empezarás con una estructura básica, añadirás cada parte siguiendo los pasos y finalmente personalizarás tu página.

## Qué aprenderás

Al terminar podrás organizar una página en secciones, relacionar sus elementos HTML con las reglas CSS, ajustar colores y espacios, y comprobar que las imágenes y los enlaces funcionen. También reconocerás qué hace un campo de texto y qué funciones todavía no tiene este proyecto.

Puedes seguir el [video de la lección 8](https://youtu.be/v4FXV4srPdA) y consultar la [presentación](lesson-8-simple-web-page-presentation.pptx). Avanza a tu ritmo y dedica el tiempo que necesites a las actividades.

## Paso 1: Abre el proyecto

Utilizaremos dos archivos:

| Archivo | Para qué sirve |
| --- | --- |
| [index.html](../../starter-files/lesson-8-simple-web-page/index.html) | Contiene la estructura inicial y comentarios que indican dónde añadir el contenido. |
| [styles.css](../../starter-files/lesson-8-simple-web-page/styles.css) | Contiene selectores con instrucciones para completar sus propiedades. |

1. Abre el [editor HTML de OneCompiler](https://onecompiler.com/html).
2. Abre el archivo `index.html` enlazado arriba. En GitHub puedes utilizar la vista **Raw** para ver solamente el código. Copia todo su contenido.
3. Reemplaza el contenido del archivo HTML del editor con ese código.
4. Haz lo mismo con `styles.css`: copia su contenido completo en el archivo CSS del editor y conserva el nombre `styles.css`.
5. Si aparece un archivo JavaScript, déjalo vacío. Esta página solo necesita HTML y CSS.
6. Ejecuta el proyecto y observa la vista previa.

Al iniciar verás una página en blanco: todavía no has añadido contenido visible ni propiedades CSS. Es el resultado esperado. Al completar la guía tendrás una tarjeta con título, pasatiempos, dos imágenes, un enlace y un campo de texto. Las imágenes necesitarán conexión a Internet porque están alojadas en otros sitios.

Si ya descargaste el proyecto, también puedes abrir `index.html` en tu navegador. Mantén `styles.css` en la misma carpeta. Después de editar y guardar un archivo, recarga la página para ver el cambio.

**Cómo seguir los pasos:** añade los fragmentos HTML debajo del comentario correspondiente, dentro de `main`. Conserva su apertura y su cierre: no crees otro `main`. En CSS, completa o sustituye cada regla vacía por la regla del mismo nombre que se muestra en la guía. Haz un cambio a la vez y vuelve a ejecutar. La carpeta `completed-examples` contiene una posible página terminada para comparar al final.

## Paso 2: Reconoce la estructura del documento

Al principio de `index.html` ya tienes la estructura siguiente. Cambia el título inicial «Mi página» por «Mi espacio creativo»:

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi espacio creativo</title>
  <link rel="stylesheet" href="styles.css">
</head>
```

Una **etiqueta** indica qué tipo de elemento estamos escribiendo. Por ejemplo, `<title>` inicia el título del documento y `</title>` lo cierra. Un **atributo** añade información dentro de una etiqueta: en `lang="es"`, `lang` es el nombre del atributo y `es` es su valor.

- `<!DOCTYPE html>` indica que el documento utiliza HTML moderno.
- `<html lang="es">` contiene la página e indica que su idioma es español. Su cierre `</html>` está al final del archivo.
- `<head>` reúne información de configuración. El contenido principal que verá el visitante está después, dentro de `<body>`.
- `charset="UTF-8"` permite interpretar correctamente caracteres como las tildes y la ñ.
- La configuración `viewport` ayuda a que el navegador móvil use el ancho del dispositivo para mostrar la página.
- `<title>` define el texto de la pestaña del navegador.
- `<link rel="stylesheet" href="styles.css">` conecta el HTML con la hoja de estilos. `href` indica dónde encontrar ese archivo.

**Prueba:** cambia solo el texto dentro de `<title>`. Si abres el HTML directamente en el navegador, cambiará el nombre de su pestaña. El título grande dentro de la página seguirá igual: lo controla otra etiqueta, que veremos en el siguiente paso. En un editor integrado, la pestaña exterior puede conservar el nombre del editor.

## Paso 3: Organiza la presentación y los títulos

Dentro de `<body>` está el contenido visible. La base ya utiliza `<main>` para agruparlo. Bajo el comentario de presentación, añade `h1` y `p` hasta obtener este inicio:

```html
<main class="tarjeta">
  <!-- 1. PRESENTACIÓN -->
  <h1>Mi espacio creativo</h1>
  <p>¡Bienvenido! Soy Alex y esta página reúne algunas cosas que me gustan.</p>
```

Este fragmento muestra el inicio del bloque; su cierre `</main>` aparece al final del contenido, antes de `</body>`.

`<h1>` es el título principal de la página y `<p>` representa un párrafo. El texto se escribe entre la etiqueta de apertura y la de cierre. Los encabezados `<h2>` del resto del archivo presentan apartados dentro del tema principal, como «Mis pasatiempos».

`class="tarjeta"` asigna una clase al elemento `main`. Más adelante, CSS utilizará ese nombre para darle fondo blanco, borde y espacios. El nombre de una clase se elige al escribir el proyecto: «tarjeta» no es una etiqueta especial de HTML.

Las líneas entre `<!--` y `-->` son comentarios. Ayudan a encontrar las tres partes del proyecto: presentación, pasatiempos e información adicional. No aparecen en la vista previa ni crean secciones visibles por sí mismas. Cuando completes una parte, puedes conservar o quitar su comentario.

**Prueba:** cambia el texto de `<h1>` por «Mi rincón favorito» y escribe una breve presentación dentro de `<p>`. Puedes inventar un personaje. Ejecuta y comprueba que aparecen ambos textos. Todavía tendrán los estilos predeterminados del navegador. Si quieres que la pestaña y el título principal coincidan, actualiza también `<title>`.

## Paso 4: Modifica la lista de pasatiempos

Añade este bloque debajo del comentario de pasatiempos, después de la presentación:

```html
<h2>Mis pasatiempos</h2>
<ul>
  <li>Leer</li>
  <li>Dibujar</li>
  <li>Escuchar música</li>
</ul>
```

`<ul>` agrupa una lista sin numeración. Cada `<li>` representa un elemento y produce una viñeta. Las tres actividades están dentro de la misma lista porque aparecen entre `<ul>` y `</ul>`.

**Prueba:** reemplaza «Leer» por «Cocinar» y ejecuta. Debe cambiar una sola viñeta. Para añadir otra actividad, coloca una línea como `<li>Bailar</li>` antes de `</ul>`.

Conserva las etiquetas de cierre y los espacios al inicio de las líneas. Esos espacios se llaman sangría: ayudan a leer qué elementos están dentro de otros, aunque no son los que generan las viñetas.

## Paso 5: Comprende las imágenes y el enlace

### Imágenes

Debajo del comentario de información adicional, añade primero `<h2>Un espacio para aprender</h2>`. Después inserta la primera imagen:

```html
<img src="https://placehold.co/360x200/png?text=Mi+espacio+creativo"
     alt="Recuadro con el texto Mi espacio creativo"/>
```

`img` inserta una imagen. `src` indica la dirección del archivo y `alt` proporciona un texto que describe su contenido. Esa descripción ayuda a quienes usan lectores de pantalla y puede mostrarse cuando la imagen no carga; no funciona como un pie de foto visible debajo de la imagen.

A diferencia de `p`, `img` no contiene texto entre una apertura y un cierre: no necesita `</img>`. La barra final que ves en el ejemplo es opcional en HTML.

Añade también una segunda imagen, una fotografía de un árbol:

```html
<img src="https://www.dzoom.org.es/wp-content/uploads/2014/07/night-810x540.jpg"
     alt="Árbol solitario reflejado en el agua bajo un cielo nocturno estrellado">
```

Cada imagen tiene su propio `src` y su propia descripción. Si sustituyes alguna, usa la dirección directa de la imagen y actualiza `alt` para que describa el nuevo contenido.

**Comprueba:** identifica cuál de las dos etiquetas corresponde a cada imagen de la vista previa. Si una no carga, revisa su dirección y tu conexión; un recurso externo también puede dejar de estar disponible.

### Enlace

Debajo de las imágenes, añade el enlace dentro de un párrafo:

```html
<p>
  <a href="https://developer.mozilla.org/es/docs/Web/HTML"
     target="_blank" rel="noopener noreferrer">Aprender HTML</a>
</p>
```

`<a>` crea un enlace. `href` contiene la dirección de destino, mientras que «Aprender HTML» es el texto visible sobre el que haces clic. `target="_blank"` abre el destino en otra pestaña o ventana, según el navegador. `rel="noopener noreferrer"` evita dar acceso a la ventana de origen y omite el envío de la dirección de procedencia al abrir el destino.

**Prueba:** cambia «Aprender HTML» por «Consultar HTML», dejando intacto `href`. Ejecuta y haz clic: cambia el texto visible, pero el destino sigue siendo la documentación de HTML.

## Paso 6: Usa el campo de texto

Añade estas líneas después del enlace, aún dentro de `main`:

```html
<label for="pasatiempo">¿Cuál es tu pasatiempo favorito?</label>
<input id="pasatiempo" type="text" placeholder="Por ejemplo: bailar">
<p class="nota">Este campo es de práctica: no guarda ni envía tu respuesta.</p>
```

`label` presenta la pregunta e `input` crea el campo. El atributo `type="text"` indica que permite escribir texto. `placeholder` muestra una pista mientras el campo está vacío; no reemplaza la pregunta.

El valor de `for` en la etiqueta y el valor de `id` en el campo coinciden: ambos dicen `pasatiempo`. Esa relación conecta la pregunta con el campo. El identificador `id` debe ser único en la página.

**Prueba:** haz clic en la pregunta y después escribe «Jugar fútbol». El campo debe recibir el foco para escribir y la pista desaparecerá al introducir texto.

Este ejemplo no guarda ni envía la respuesta y tampoco la añade a la lista de arriba. Para cambiar esa lista, debes editar sus elementos `li`. El párrafo con la clase `nota` explica esta limitación al visitante.

## Paso 7: Lee las reglas de CSS

Abre `styles.css`. Encontrarás selectores con comentarios, pero todavía sin propiedades. Completa la regla `h1` con este ejemplo. Una regla CSS tiene un selector y un bloque de propiedades:

```css
h1 {
  color: #2458e8;
}
```

El **selector** `h1` elige los títulos principales. Entre las llaves, `color` es la propiedad y `#2458e8` es su valor, un tono azul expresado como código hexadecimal. Los dos puntos separan propiedad y valor; el punto y coma termina la declaración.

**Prueba:** sustituye `#2458e8` por `purple`, conservando los dos puntos y el punto y coma. Ejecuta: el título se vuelve morado, pero su texto no cambia. Puedes indicar colores con nombres como `purple` o con códigos como el del ejemplo.

### Fondo y tipografía

Completa ahora la regla `body`:

```css
body {
  background: #eef4fb;
  font-family: Arial, sans-serif;
  color: #25364c;
  line-height: 1.5;
}
```

`background` establece aquí el fondo azul claro. `font-family` elige Arial y, si no está disponible, una fuente de la familia genérica `sans-serif`. `color` define el color base del texto y `line-height: 1.5` establece una altura de línea equivalente a 1,5 veces el tamaño de la fuente, para separar las líneas.

Muchos elementos reciben la fuente y el color del elemento que los contiene. Por eso estas reglas en `body` afectan al texto de la página. El título tiene su propio color porque la regla de `h1` lo define directamente.

**Prueba:** cambia temporalmente el fondo a `white`, ejecuta y observa la diferencia. Luego restaura `#eef4fb`. El contenido HTML debe permanecer igual.

## Paso 8: Da forma a la tarjeta

Completa la regla `.tarjeta` con estas propiedades. El punto indica que seleccionamos los elementos con `class="tarjeta"`:

```css
.tarjeta {
  max-width: 650px;
  margin: 32px auto;
  padding: 28px;
  background: white;
  border: 1px solid #ccd8e8;
  border-radius: 14px;
}
```

| Propiedad | Qué hace en este proyecto |
| --- | --- |
| `max-width: 650px` | Limita el ancho del contenido a 650 píxeles. En esta tarjeta, el espacio interior y el borde se suman a ese ancho. |
| `margin: 32px auto` | Deja 32 píxeles fuera de la tarjeta arriba y abajo. Los márgenes laterales automáticos la centran cuando hay espacio disponible. |
| `padding: 28px` | Deja 28 píxeles dentro, entre el contenido y el borde. |
| `background: white` | Da fondo blanco a la tarjeta. |
| `border: 1px solid #ccd8e8` | Dibuja un borde de un píxel, continuo y de color gris azulado. |
| `border-radius: 14px` | Redondea las esquinas. |

La diferencia entre `margin` y `padding` se entiende imaginando una caja: `margin` deja espacio alrededor de la caja y `padding` separa lo que hay dentro de sus paredes.

**Prueba:** cambia `padding: 28px` a `padding: 0` y ejecuta. El contenido quedará junto al borde. Después restaura `28px`. Ahora cambia el primer valor de `margin` de `32px` a `60px`: aumentará el espacio exterior vertical. Restaura el valor al terminar la comparación.

## Paso 9: Adapta las imágenes y el campo

Completa la regla `img` para que las imágenes compartan estos estilos:

```css
img {
  width: 360px;
  max-width: 100%;
  height: auto;
}
```

`width` propone un ancho de 360 píxeles. `max-width: 100%` impide que ese ancho supere el espacio disponible en el contenedor. `height: auto` ajusta la altura conservando la proporción de la imagen.

**Prueba:** reduce el ancho de la vista previa o de la ventana del navegador. Cuando el espacio de la tarjeta sea menor que 360 píxeles, las imágenes deben reducirse sin deformarse ni sobresalir.

Completa la regla `input` para dar estas propiedades al campo de texto:

```css
input {
  box-sizing: border-box;
  width: 100%;
  padding: 10px;
  border: 1px solid #66768c;
  border-radius: 6px;
  font: inherit;
}
```

`width: 100%` ocupa el ancho disponible. `box-sizing: border-box` hace que ese ancho incluya el relleno y el borde del campo. `padding`, `border` y `border-radius` funcionan como en la tarjeta, y `font: inherit` toma la configuración de fuente del elemento que lo contiene.

Completa las tres reglas restantes:

```css
a {
  color: #1745bf;
}

label {
  display: block;
  margin-bottom: 8px;
}

.nota {
  font-size: 14px;
}
```

`a` da color a los enlaces. `label` utiliza `display: block` para colocar la pregunta en su propio bloque y `margin-bottom` para separarla del campo. `.nota` selecciona el párrafo de aviso y le da un tamaño de letra de 14 píxeles.

## Paso 10: Comprueba la página

Antes de considerar terminado el proyecto, revisa lo siguiente:

- El título y la presentación se leen correctamente.
- Cada pasatiempo aparece como una viñeta independiente.
- Las dos imágenes cargan y tienen descripciones `alt` apropiadas.
- El enlace abre la documentación esperada.
- Al pulsar la pregunta, puedes escribir en el campo.
- El texto y las imágenes caben al reducir el ancho de la ventana.

Para distinguir HTML de CSS, guarda una copia del contenido de `styles.css` y vacía temporalmente ese archivo en el editor. Ejecuta: se mantienen el texto, las imágenes y el campo, pero desaparecen tus colores y espacios. El navegador sigue aplicando sus estilos predeterminados. Restaura el CSS y ejecuta otra vez.

Si algo no funciona, utiliza esta tabla para revisar el proyecto:

| Problema | Qué revisar |
| --- | --- |
| No aparecen los estilos | El HTML debe enlazar `styles.css` y el archivo CSS debe tener exactamente ese nombre. |
| No cambia el título visible | Modifica `h1`; `title` corresponde a la pestaña del navegador. |
| Un color no se aplica | Revisa el selector, los dos puntos, el valor, el punto y coma y las llaves de la regla. |
| Una imagen no carga | Comprueba `src`, la conexión y la disponibilidad del archivo externo. |
| La imagen sobresale de la tarjeta | Comprueba que la regla `img` conserve `max-width: 100%`. |
| Pulsar la pregunta no activa el campo | Verifica que `for` e `id` tengan el mismo valor. |
| No aparecen tus últimos cambios | Guarda y recarga si trabajas localmente, o vuelve a ejecutar el proyecto en el editor. |

## Paso 11: Personaliza tu página

Una vez construida la página, realiza este reto de personalización. Si ya hiciste cambios durante la guía, puedes aprovecharlos:

1. Elige un título propio y escríbelo en `h1`. Actualiza también `title` para mantener el mismo nombre en la pestaña.
2. Escribe tres pasatiempos diferentes dentro de los elementos `li`.
3. Cambia el color del título en la regla CSS de `h1`.
4. Cambia el texto visible del enlace, conservando su dirección `href`.

Puedes utilizar datos inventados. Como desafío opcional, añade un cuarto pasatiempo y explica con tus palabras la diferencia entre `margin` y `padding`.

Tu reto estará completo si aparecen tu nuevo título y tus pasatiempos, el título tiene otro color y el enlace muestra otro texto sin cambiar de destino. Los colores y las palabras no necesitan coincidir con los de la solución.

## Compara con una posible solución

Cuando termines, consulta el [HTML resuelto](../../completed-examples/lesson-8-simple-web-page/index.html) y su [CSS](../../completed-examples/lesson-8-simple-web-page/styles.css). Ambos archivos contienen la página completa, con el reto de personalización resuelto.

La solución utiliza «Mi mundo de pasatiempos», un título morado y el enlace «Consultar la guía de HTML». Muestra cuatro pasatiempos porque incluye el desafío opcional. También actualiza el texto de la imagen de muestra para que coincida con el nuevo título; este es un ajuste adicional.

Antes de cerrar la lección, comprueba que puedes responder: ¿dónde cambiarías el contenido de la página?, ¿qué regla controla el color del título?, ¿qué diferencia hay entre `src` y `href`?, ¿por qué coinciden `for` e `id`? Si alguna respuesta no está clara, vuelve al paso correspondiente y prueba un cambio pequeño en el proyecto.
