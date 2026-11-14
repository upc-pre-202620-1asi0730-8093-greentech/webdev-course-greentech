# Lección 6 Propiedades de CSS

- **Duración máxima del video:** 7 minutos.
- **Objetivo de grabación:** entre 6:40 y 6:50; nunca superar 7:00.
- **Público:** estudiantes de secundaria sin experiencia previa.
- **Resultado:** una tarjeta de pasatiempos con texto legible, colores y espacios.

## Materiales

- [Presentación](lesson-6-css-properties-presentation.pptx).
- [HTML inicial](../../starter-files/lesson-6-css-properties/index.html) y [CSS inicial preparado](../../starter-files/lesson-6-css-properties/styles.css).
- [HTML resuelto](../../completed-examples/lesson-6-css-properties/index.html) y [CSS resuelto](../../completed-examples/lesson-6-css-properties/styles.css).

Se conserva la secuencia del Word de referencia: explicación breve, ejemplo preparado, comprobación y reto. El guion distingue lo que se dice de las acciones de grabación.

## Preparación antes de grabar

Abrir un editor HTML y CSS en el navegador, como el utilizado en las otras lecciones del curso. No hace falta instalar un editor. Cargar el HTML en la sección HTML y el contenido de `styles.css` en la sección CSS. Si el editor trabaja con archivos completos, conservar el enlace a `styles.css`; si usa paneles separados y enlaza el CSS automáticamente, retirar ese enlace de la copia pegada en el panel HTML.

Preparar una pestaña de trabajo con el HTML y el CSS iniciales. La solución queda abierta únicamente como referencia para comprobar el resultado al terminar; no se copia durante la demostración. Mostrar código y resultado a la vez, con un tamaño de letra que se lea en la grabación. No gastar tiempo creando archivos o escribiendo todo el ejemplo. Los cambios pequeños de valores sí se realizan durante la demostración.

La clase `card` y el HTML ya están preparados. No explicar todavía cómo funcionan los selectores: ese tema pertenece a la lección 7. `max-width` solo limita el ancho del ejemplo y no requiere desarrollar un tema adicional.

## Cronograma de referencia

Los intervalos incluyen narración, movimientos del cursor, cambios de ventana y comprobaciones. No corresponden a minutos de lectura continua. Las portadas entran en la introducción y no agregan tiempo.

| Intervalo máximo | Contenido | Qué se muestra |
| --- | --- | --- |
| 00:00–00:35 | Introducción | Portada y tarjeta inicial. |
| 00:35–00:55 | Color y fondo | Diapositiva de color. |
| 00:55–01:40 | Demostración de colores | Editor y resultado. |
| 01:40–02:05 | Fuente y tamaño | Diapositiva de tipografía. |
| 02:05–02:45 | Demostración de texto | Editor y resultado. |
| 02:45–03:15 | Espacio exterior e interior | Diapositiva de espacios. |
| 03:15–04:10 | Demostración de tarjeta | Editor y resultado. |
| 04:10–05:50 | Comparaciones | Editor y resultado, sin otra explicación extensa. |
| 05:50–06:40 | Reto independiente | Diapositiva de actividad y archivo inicial. |
| 06:40–07:00 | Cierre | Resultado final. Terminar preferiblemente antes de 6:50. |

Las diapositivas con la indicación «cambiar al editor» son guías del presentador. Se usa el editor real en esos tramos; no se leen las indicaciones técnicas al estudiante.

## Guion para la grabación

### 00:00–00:35 Introducción

**Narración**

Esta tarjeta ya tiene un título y dos párrafos. También tiene estilos preparados, pero sus colores y espacios son sencillos. Durante la lección cambiarán unos pocos valores para darle una apariencia más clara. El contenido seguirá siendo el mismo. Cada cambio se comprobará en la vista previa.

**Acciones para grabar:** mostrar la portada y después la pestaña de trabajo. Abrir el panel HTML y señalar el título y los dos párrafos sin editarlos. Abrir el CSS y ejecutar la vista previa. Debe aparecer una tarjeta blanca con borde gris, esquinas rectas y poco espacio interior. No mostrar una solución distinta como si fuera el archivo de trabajo.

### 00:35–00:55 Color y fondo

**Narración**

`color` cambia el color del texto. `background-color` cambia el fondo. Piensa en una hoja y un lápiz: una cosa es el color de la hoja y otra, el de las letras. Conviene elegir colores que permitan leer con facilidad.

**Acción:** señalar las dos propiedades de la diapositiva.

### 00:55–01:40 Demostración de colores

**Narración**

El ejemplo ya tiene un fondo gris claro. En el bloque body, background-color controla el fondo de la página. Al cambiarlo por este azul claro, la tarjeta blanca se distingue mejor. Ahora el título también puede recibir un color propio. La propiedad color cambia sus letras, sin cambiar lo que dicen. Los códigos que empiezan con almohadilla representan colores.

**Acciones para grabar, en este orden:**

1. Abrir el panel CSS y localizar el primer bloque, `body`.
2. Cambiar únicamente `background-color: #f4f4f4;` por `background-color: #eef4ff;`. Ejecutar o actualizar la vista previa. Señalar el fondo exterior azul claro.
3. Localizar `h1`. Cambiar `color: #25364c;` por `color: #2458e8;`. Conservar el color de `p`.
4. Ejecutar y señalar el título azul. Dejar ambos cambios aplicados; no restaurar los valores iniciales.

### 01:40–02:05 Fuente y tamaño

**Narración**

La fuente es la forma de las letras. `font-family` permite elegirla y `font-size` controla su tamaño. Un texto puede verse bonito y aun así ser difícil de leer si sus letras son demasiado pequeñas. La lectura debe resultar cómoda.

**Acción:** mostrar el concepto y regresar al editor.

### 02:05–02:45 Demostración de texto

**Narración**

Las letras del ejemplo tienen inicialmente otra forma. Al elegir Arial cambia la fuente de la página. Los párrafos empiezan con dieciséis píxeles; al subir a dieciocho, se ven más grandes. Después aumenta el espacio entre sus líneas. Son tres cambios distintos: forma, tamaño y separación. No hace falta cambiar el texto para mejorar su lectura.

**Acciones para grabar:**

1. En `body`, sustituir `font-family: Georgia, serif;` por `font-family: Arial, sans-serif;`. Ejecutar y señalar la forma de las letras.
2. En `p`, sustituir `font-size: 16px;` por `font-size: 18px;`. Ejecutar y observar el tamaño de los párrafos.
3. En el mismo bloque, sustituir `line-height: 1.3;` por `line-height: 1.5;`. Ejecutar y señalar la separación entre líneas. Si un párrafo ocupa una sola línea, estrechar ligeramente la vista previa para observarlo.
4. Mantener los tres valores finales.

### 02:45–03:15 Espacios y borde

**Narración**

El borde marca el contorno de la tarjeta. `padding` deja espacio dentro, entre el texto y el borde. `margin` deja espacio fuera y la separa de lo que tiene alrededor. Una forma de recordarlo es pensar en una caja: el relleno está dentro y la separación con otras cajas está fuera.

**Acción:** señalar el contenido, el espacio interior y el exterior en la diapositiva. Evitar explicar todas las variantes de cada propiedad.

### 03:15–04:10 Demostración de tarjeta

**Narración**

El bloque card reúne los estilos de la tarjeta. Primero aumenta el margen exterior: la tarjeta baja un poco y conserva su posición centrada. Después aumenta el espacio interior: las letras se alejan del borde. El borde ya existe; ahora cambia su color. Por último, las esquinas pasan de rectas a redondeadas. Cada propiedad tiene un efecto diferente.

**Acciones para grabar:** localizar `.card` en CSS y realizar un cambio por vez, ejecutando después de cada uno.

| Orden | Valor inicial | Valor final | Qué señalar en la vista previa |
| --- | --- | --- | --- |
| 1 | `margin: 8px auto;` | `margin: 20px auto;` | Mayor espacio sobre y debajo de la tarjeta. `auto` ya estaba preparado para centrarla. |
| 2 | `padding: 8px;` | `padding: 24px;` | Separación entre las letras y el borde. |
| 3 | `border: 2px solid #999999;` | `border: 2px solid #486bba;` | El borde gris se vuelve azul. Mantener su grosor. |
| 4 | `border-radius: 0;` | `border-radius: 12px;` | Esquinas redondeadas. |

No escribir reglas nuevas ni cambiar el HTML. `max-width` y el fondo blanco ya están preparados.

### 04:10–05:50 Pruebas y comparación

**Narración**

Ahora compara tres detalles. Primero, el tamaño del texto: debe leerse sin acercarse demasiado a la pantalla. Después, el espacio interior: el contenido necesita separarse del borde. Por último, los colores: un texto oscuro sobre un fondo claro se distingue mejor que dos colores muy parecidos. También puedes alinear el título al centro con `text-align`. Cambia una propiedad a la vez y comprueba el resultado antes de continuar. Así resulta más fácil reconocer qué hizo cada cambio.

**Acción:** realizar tres comparaciones breves: `font-size: 18px` frente a `12px`; `padding: 24px` frente a `0`; color oscuro frente a uno demasiado claro. Restaurar los valores de la solución. Mostrar `text-align: center` en el título. Este tramo reserva tiempo para observar los resultados, no para añadir propiedades nuevas. Si la grabación va retrasada, reducir las repeticiones y pasar al reto.

### 05:50–06:40 Reto

**Narración**

Ahora puedes personalizar tu tarjeta. El HTML ya está preparado: no necesitas empezar desde cero. Cambia el fondo y elige una fuente. Después, personaliza el borde y el espacio interior con `padding`. Comprueba que el texto se lea bien. Como desafío adicional, separa la tarjeta con `margin` y redondea sus esquinas. Pausa el video para completar la actividad y compara tu resultado con la solución cuando termines. Tu tarjeta puede tener otros colores y seguir siendo correcta.

**Acción:** mostrar la diapositiva del reto. Indicar que se puede descargar una copia nueva del ejemplo inicial para practicar, conservando aparte el trabajo realizado. No resolver el ejercicio en el video ni esperar a que el estudiante lo termine.

### 06:40–07:00 Cierre

**Narración**

Ya conoces propiedades para mejorar tu tarjeta. La siguiente lección explica cómo elegir qué elementos reciben cada estilo.

**Acción:** mostrar la tarjeta final y detener la grabación. No agregar despedidas o recapitulaciones adicionales después del límite.

## Criterios del reto

La tarjeta debe conservar su título y párrafos. Debe incluir un fondo, una fuente legible, un borde y espacio interior. Los colores y el texto pueden personalizarse; no tienen que coincidir con la solución. `margin` y `border-radius` son mejoras adicionales.

## Control de duración

Realizar un ensayo con cronómetro antes de grabar. Si un bloque supera su intervalo, recortar la explicación o repetir menos cambios; no hablar más rápido para compensarlo. La narración por sí sola no garantiza la duración final: el ensayo debe incluir las demostraciones. La actividad se resuelve con el video pausado y no añade tiempo a la grabación.

## Referencias

- [Espacio interior con padding en MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/padding).

## Hoja de control para el presentador

Las instrucciones de acción y las tablas no se leen en voz alta. Leer solo los párrafos de **Narración** y usar las acciones como recordatorio. No leer los códigos hexadecimales carácter por carácter: señalar el valor y decir «este azul claro» o «este color oscuro».

Antes de iniciar la grabación en Windows:

1. Descargar o actualizar el repositorio y abrir las carpetas de esta lección. No combinar el HTML inicial con el CSS resuelto.
2. Abrir el editor del curso en el navegador; cargar ambos archivos iniciales. Comprobar que el CSS se aplica antes de grabar. Mantener JavaScript vacío.
3. Abrir la presentación y el guion en otra pantalla o dispositivo. Desactivar notificaciones y aumentar el tamaño del código hasta que resulte legible.
4. Ensayar los cambios con cronómetro. Al terminar, volver a cargar los archivos iniciales antes de la toma definitiva.
5. Durante las demostraciones, mostrar el editor real. Las diapositivas ocultas «CAMBIAR AL EDITOR» sirven como recordatorio, no como pantalla del video.

Al finalizar la demostración de tarjeta, las nueve sustituciones deben producir exactamente el CSS de la carpeta completed-examples. El HTML no cambia. Las pruebas del tramo 04:10–05:50 son temporales: restaurar tamaño a 18px, padding a 24px y color de párrafos a #25364c antes del reto. Dejar unos segundos para observar cada resultado, sin leer todo el archivo.

**Si falla algo durante la toma:** comprobar que el cambio está en el bloque indicado, que conserva los dos puntos y el punto y coma, y ejecutar la vista previa. Detener y repetir el tramo si hace falta; no dedicar el tiempo de la clase a buscar archivos o configurar el editor. Las pausas para resolver el reto las realiza el estudiante fuera del tiempo del video.
