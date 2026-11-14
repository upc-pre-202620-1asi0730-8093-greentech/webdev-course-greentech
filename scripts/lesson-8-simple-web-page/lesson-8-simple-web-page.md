# Lección 8: Página web sencilla

Persona 5 · Grabación de aproximadamente 12 minutos.

Basado en el Word «Guiones_Companeros_Web_Metodo_Dinamico» y en las diapositivas 55 a 71 de «Curso_Web_Presentaciones_Companeros_Completo».

## Materiales del repositorio

- [Presentación de la lección 8](lesson-8-simple-web-page-presentation.pptx).

- [Página inicial](../../starter-files/lesson-8-simple-web-page/index.html).
- [Estilos iniciales](../../starter-files/lesson-8-simple-web-page/styles.css).
- [Reto independiente](../../starter-files/lesson-8-simple-web-page/Reto_independiente.md).
- [Página resuelta](../../completed-examples/lesson-8-simple-web-page/index.html).
- [Estilos de la solución](../../completed-examples/lesson-8-simple-web-page/styles.css).
- [Explicación de la solución](../../completed-examples/lesson-8-simple-web-page/Solucion.md).

Para la demostración, utiliza el HTML y el CSS de starter-files de esta lección. La solución muestra una posible personalización e incluye el cuarto pasatiempo opcional.

## Antes de grabar

1. Abre https://onecompiler.com/html (sin la coma del enlace original).
2. Copia el contenido de `index.html` en la pestaña HTML del editor y el de `styles.css` en la pestaña `styles.css`. Reemplaza el ejemplo inicial. Si hay código en `scripts.js`, déjalo vacío: esta lección no necesita JavaScript.
3. Ejecuta el ejemplo con el control de ejecución del editor. Debes ver una tarjeta blanca, un título azul, tres pasatiempos, dos imágenes, un enlace y un campo de texto.
4. Prepara otra pestaña de OneCompiler con el mismo HTML, pero con `styles.css` completamente vacío. Será la versión «sin nuestros estilos». El navegador seguirá mostrando sus estilos predeterminados.
5. Comprueba antes de grabar que las dos imágenes carguen y que el enlace abra MDN. Las imágenes necesitan conexión a Internet. Si alguna no carga, revisa su dirección y vuelve a ejecutar.
6. Aumenta el zoom hasta que el código se lea en tu grabación. Mantén visibles el código y el resultado. Cierra notificaciones y pestañas innecesarias.
7. Ensaya con cronómetro. Los intervalos incluyen narración, desplazamientos, demostraciones y pequeñas pausas. Leer el texto seguido tardará menos de 12 minutos.

El material pide código preparado. Durante la grabación, señala los fragmentos y muestra el resultado. Solo necesitas escribir dentro del campo de práctica. Puedes usar el PowerPoint para introducir conceptos; las diapositivas que dicen «GUÍA PARA EL PRESENTADOR · NO GRABAR» se sustituyen por el editor real.

## Guion: qué decir y qué mostrar

Las acciones entre corchetes son indicaciones para ti: no las leas en voz alta. Los textos entre comillas son una base para hablar con naturalidad.

### 00:00–00:45 · Presentación del proyecto

[Muestra el resultado terminado. Recorre con el cursor el título, la lista, las imágenes y el campo.]

«Hola, soy Diego y en esta lección vamos a reunir lo que hemos aprendido de HTML y CSS en una página sencilla. Nuestro ejemplo se llama Mi espacio creativo. Tiene una presentación, una lista de pasatiempos, dos imágenes, un enlace para aprender más y un espacio para escribir. El código ya está preparado en OneCompiler. Vamos a revisar qué hace cada parte y a relacionarla con lo que aparece en pantalla. Al terminar, podrás personalizar esta página con tus propias ideas».

### 00:45–01:10 · Organización de la página

[Señala los tres comentarios numerados del HTML.]

«Antes de pensar en colores, organizamos la información. Aquí tenemos tres partes: una presentación, nuestros pasatiempos y una sección con información adicional. Es parecido a organizar una hoja antes de decorarla. Estos comentarios nos ayudan a encontrar cada parte en el código, pero no se muestran en la página».

### 01:10–02:10 · Título y presentación

[Señala `main`, `class="tarjeta"`, `h1` y `p`. Después señala sus resultados.]

«Empezamos por main, que contiene el contenido principal de nuestra página. Dentro encontramos h1: esta etiqueta identifica el título principal. El texto que está entre la apertura y el cierre es lo que aparece aquí: Mi espacio creativo. Debajo usamos p para escribir un párrafo de bienvenida».

[Selecciona solamente el texto del título y después su etiqueta de cierre.]

«Observa que el cierre lleva una barra. Así indicamos dónde termina el título. El párrafo tiene su propia apertura y cierre. También aparece class igual a tarjeta. Le estamos dando un nombre que luego utilizaremos en CSS para aplicar estilos a este bloque. Poner esa clase por sí solo todavía no crea el fondo blanco: eso lo hace el CSS que veremos después».

[Deja unos segundos para comparar el código con el título y el párrafo visibles.]

### 02:10–02:30 · Qué es una lista

[Señala las viñetas en el resultado.]

«Para mostrar nuestros pasatiempos usamos una lista. Como no son pasos que debamos seguir en orden, elegimos ul, una lista sin numeración. Dentro, cada pasatiempo se escribe con li. Por eso vemos una viñeta al lado de cada actividad».

### 02:30–03:30 · Revisar los pasatiempos

[Muestra el bloque desde `h2` hasta `</ul>`. Señala un `li` y su viñeta, de uno en uno.]

«Este h2 presenta el apartado Mis pasatiempos. Es un título de sección que está dentro del tema principal. Después empieza ul y dentro aparecen tres elementos li: leer, dibujar y escuchar música. Cada uno corresponde a una línea de la lista que vemos a la derecha».

«Si quisiéramos añadir bailar, colocaríamos otro li dentro de esta misma lista. Si solo quisiéramos cambiar leer por cocinar, cambiaríamos ese texto. La estructura puede quedarse igual. Fíjate también en los espacios al inicio de las líneas: nos ayudan a reconocer qué elementos están dentro de otros».

[Señala dónde iría el cuarto elemento sin escribirlo. Recorre las aperturas y cierres.]

«Entonces, ul reúne la lista completa y li representa cada elemento de esa lista».

### 03:30–03:55 · Imagen y enlace

[Señala `img` y luego `a`.]

«Ahora revisamos las imágenes y el enlace. Para cada imagen usamos img. **Su atributo src indica dónde está la imagen**, y **alt describe la imagen mediante texto**. Para el enlace usamos a. Su atributo **href indica la dirección que se abrirá cuando hagamos clic**».

### 03:55–05:05 · Revisar los recursos

[Señala brevemente la primera imagen de muestra. Después selecciona el `src` de la segunda imagen, la fotografía del árbol, y señala su resultado.]

«Conservé la imagen de muestra y añadí esta fotografía que encontré buscando en Google. Copié la dirección de la imagen en src. Google me ayudó a encontrarla; el archivo está alojado en dZoom. Debemos copiar la dirección de la imagen, no la de los resultados de búsqueda».

[Señala `alt="Árbol solitario reflejado en el agua bajo un cielo nocturno estrellado"`.]

«En alt describí lo que vemos: un árbol solitario reflejado en el agua bajo un cielo nocturno estrellado. Este texto ayuda a quienes usan lectores de pantalla y también puede aparecer si la foto no carga. Alt describe el contenido; no es el nombre del archivo».

[Señala la dirección de `href` y el texto «Aprender HTML».]

«En el enlace, href indica el destino: la documentación de MDN. Aprender HTML es el texto que vemos. Vamos a comprobarlo».

[Abre el enlace. Muestra brevemente la página de destino y regresa al editor.]

«**Target con el valor _blank abre el enlace en otra pestaña o ventana, según el navegador**. **Recuerda: src indica dónde está la imagen y href indica el destino del enlace**».

### 05:05–05:25 · Campo de texto

[Señala el campo y su pregunta.]

«También podemos dejar un espacio para escribir. **Label presenta la pregunta y el input de tipo text permite introducir una respuesta**. En este ejemplo solo practicamos la escritura: no hemos programado una función para guardar ni enviar lo que escribimos».

### 05:25–06:15 · Probar el campo

[Señala `for="pasatiempo"` y `id="pasatiempo"`.]

«**Estas dos palabras coinciden: el for de label y el id del input dicen pasatiempo. Esa coincidencia conecta la pregunta con el campo. Podemos comprobarlo haciendo clic en la pregunta: el cursor pasa al espacio para escribir**».

[Haz clic en la etiqueta y escribe «Jugar fútbol» en el campo.]

«**Ahora puedo escribir mi respuesta. El texto gris que aparecía antes era una pista, llamada placeholder. La pista desaparece cuando escribo, pero la pregunta sigue visible. Y recuerda: escribir aquí no añade un nuevo pasatiempo a la lista de arriba ni lo guarda. Es únicamente un campo de práctica**».

### 06:15–06:35 · Relación entre HTML y CSS

[Muestra la pestaña sin estilos y vuelve a la versión terminada.]

«**Hasta aquí hemos hablado del contenido. HTML organiza lo que hay en la página. CSS define cómo se presenta. En estas dos versiones tenemos el mismo contenido, pero una usa nuestros colores, espacios y bordes. Vamos a ver las reglas que producen esa diferencia**».

### 06:35–08:00 · Fondo, tarjeta y espacios

[Abre `styles.css`. Señala `body` y sus propiedades, después `.tarjeta`.]

«La regla body aplica estilos al cuerpo de la página. Background define el fondo azul claro y font-family elige Arial como fuente, con una alternativa genérica si no está disponible. Color establece el color del texto y line-height deja una separación cómoda entre las líneas».

«Después encontramos punto tarjeta. Ese punto indica que estamos seleccionando una clase. Es la misma clase tarjeta que vimos en main, dentro del HTML».

[Vuelve un momento al HTML para señalar la clase; regresa al CSS.]

«Max-width limita el ancho del contenido de la tarjeta a 650 píxeles. Margin deja espacio por fuera: aquí usamos 32 píxeles arriba y abajo, y auto a los lados para centrarla cuando sobra espacio. Padding deja espacio por dentro: separa el texto del borde. Background white le da el fondo blanco».

[Señala en la vista previa el espacio fuera y dentro de la tarjeta.]

«Para recordarlo, imagina una caja: margin deja separación alrededor de la caja y padding deja espacio entre el contenido y su borde. Son espacios distintos».

### 08:00–08:30 · Bordes e imagen adaptable

[Señala las esquinas y luego la imagen.]

«Los detalles también ayudan a que la página se entienda. El borde permite distinguir la tarjeta del fondo y las esquinas redondeadas cambian su apariencia. Además, queremos que la imagen quepa si el espacio disponible se hace más pequeño. Para eso limitamos su ancho y conservamos sus proporciones».

### 08:30–09:50 · Revisar los detalles finales

[Señala `border`, `border-radius`, la regla `h1` y la regla `img`.]

«Border tiene tres partes: un píxel de grosor, una línea continua indicada por solid y el color del borde. Border-radius redondea las esquinas. En h1, la propiedad color hace que el título principal se vea azul».

«En img tenemos max-width al cien por ciento. Eso limita la imagen al ancho disponible en su contenedor y evita que sobresalga. Height auto permite que su altura se ajuste manteniendo la proporción. Así la imagen no se estira de forma extraña».

[Reduce el ancho disponible para el resultado, sin ocultarlo. Observa cómo se redistribuye el texto y cómo se reduce la imagen si el espacio es menor que su ancho.]

«Al reducir el espacio, el texto puede ocupar más líneas y la imagen puede hacerse más pequeña. Esto nos ayuda a mantener la página legible».

[Restaura el ancho. Señala brevemente las reglas de `label` e `input`.]

«Las últimas reglas dan espacio a la pregunta y al campo para que sea cómodo escribir. No necesitamos memorizar todo: lo importante es reconocer qué elemento seleccionamos y qué propiedad cambia su apariencia».

### 09:50–10:50 · Comprobación del resultado

[Haz cada comprobación mientras la mencionas.]

«Vamos a revisar nuestra página como si fuéramos sus visitantes. Primero, el título nos dice de qué trata. Segundo, los tres pasatiempos se leen como una lista. Las dos imágenes cargan y el enlace nos lleva al recurso esperado, como comprobamos antes. También podemos hacer clic en la pregunta y escribir en el campo».

[Alterna entre la versión sin estilos y la versión con estilos.]

«Ahora comparemos. En ambas aparecen el mismo título, la misma lista, las imágenes y el campo. Lo que cambia es su presentación. Sin nuestro CSS, el navegador usa su aspecto predeterminado. Con nuestro CSS, vemos el fondo, la tarjeta, los colores y los espacios que elegimos. Esta comparación nos permite distinguir el trabajo de HTML del trabajo de CSS».

### 10:50–11:40 · Actividad para el estudiante

[Muestra `Reto_independiente.md` o la diapositiva de actividad.]

«Ahora te toca personalizar el ejemplo. Cambia el título por uno que te guste. Escribe tres pasatiempos diferentes. Después cambia el color del título y modifica las palabras visibles del enlace. Puedes utilizar un personaje o datos inventados».

«Una pista: el título y los pasatiempos están en HTML. El color está en CSS, dentro de la regla h1. Para cambiar lo que dice el enlace, busca el texto entre la apertura y el cierre de a».

«Cuando termines, ejecuta el ejemplo y comprueba que tus cambios se vean. Pausa el video para realizar la actividad y continúa cuando estés listo».

[Haz una pausa breve. No hace falta esperar a que el alumno resuelva el ejercicio dentro de tu grabación.]

### 11:40–12:00 · Cierre

[Muestra la página terminada.]

«Hoy reunimos los elementos principales de HTML y CSS en una página sencilla. Organizamos el contenido, le dimos estilo y comprobamos el resultado. Ya puedes usar esta misma estructura para crear una página sobre tus intereses. Con esto terminamos la lección 8. ¡Gracias!».

## Recordatorio rápido para hablar sin memorizar

Sigue esta secuencia en cada demostración: **qué hace → dónde está en el código → cómo se ve → comprobación**.

| Código | Explicación sencilla |
|---|---|
| `main` | Contenido principal de la página. |
| `h1` / `h2` | Título principal / título de una sección. |
| `p` | Párrafo. |
| `ul` / `li` | Lista sin numeración / cada elemento. |
| `src` / `alt` | Dirección de la imagen / texto que la describe. |
| `href` | Destino del enlace. |
| `label` / `input` | Pregunta o etiqueta / campo para escribir. |
| `for` e `id` | Deben coincidir para conectar etiqueta y campo. |
| `.tarjeta` | Selecciona los elementos con la clase tarjeta. |
| `margin` / `padding` | Espacio exterior / espacio interior. |
| `border` / `border-radius` | Borde / redondeo de esquinas. |
| `max-width` | Límite de ancho. |

Si te trabas, vuelve a «esta parte sirve para…» y señala el resultado. Evita leer los símbolos y las direcciones completas. Practica especialmente margin/padding y for/id: suelen necesitar una demostración visual.

Los 12 minutos son una referencia del material original. Ajusta el ritmo después de un ensayo; no alargues silencios para completar el tiempo.
