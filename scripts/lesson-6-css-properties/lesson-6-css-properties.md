# Lección 6 Propiedades de CSS

- **Duración máxima del video:** 7 minutos.
- **Objetivo de grabación:** entre 6:40 y 6:50; nunca superar 7:00.
- **Público:** estudiantes de secundaria sin experiencia previa.
- **Resultado:** una tarjeta de pasatiempos con texto legible, colores y espacios.

## Materiales

- [Presentación](lesson-6-css-properties-presentation.pptx).
- [HTML inicial](../../starter-files/lesson-6-css-properties/index.html) y [CSS para completar](../../starter-files/lesson-6-css-properties/styles.css).
- [HTML resuelto](../../completed-examples/lesson-6-css-properties/index.html) y [CSS resuelto](../../completed-examples/lesson-6-css-properties/styles.css).

Se conserva la secuencia del Word de referencia: explicación breve, ejemplo preparado, comprobación y reto. El guion distingue lo que se dice de las acciones de grabación.

## Preparación antes de grabar

Abrir un editor HTML y CSS en el navegador, como el utilizado en las otras lecciones del curso. No hace falta instalar un editor. Cargar el HTML en la sección HTML y el contenido de `styles.css` en la sección CSS. Si el editor trabaja con archivos completos, conservar el enlace a `styles.css`; si usa paneles separados y enlaza el CSS automáticamente, retirar ese enlace de la copia pegada en el panel HTML.

Preparar dos pestañas: una con el ejercicio inicial y otra con la solución. Mostrar código y resultado a la vez, con un tamaño de letra que se lea en la grabación. No gastar tiempo creando archivos o escribiendo todo el ejemplo. Los cambios pequeños de valores sí se realizan durante la demostración.

La clase `card` y el HTML ya están preparados. No explicar todavía cómo funcionan los selectores: ese tema pertenece a la lección 7. `max-width` solo limita el ancho del ejemplo y no requiere desarrollar un tema adicional.

## Cronograma de referencia

Los intervalos incluyen narración, movimientos del cursor, cambios de ventana y comprobaciones. No corresponden a minutos de lectura continua. Las portadas entran en la introducción y no agregan tiempo.

| Intervalo máximo | Contenido | Qué se muestra |
| --- | --- | --- |
| 00:00–00:35 | Introducción | Portada y tarjeta inicial frente a la final. |
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

Esta tarjeta ya tiene un título y dos párrafos, pero su apariencia todavía es sencilla. Con CSS puedes cambiar sus colores, el tamaño de las letras y los espacios. Observa la versión final: el contenido es el mismo, aunque ahora resulta más fácil distinguirlo y leerlo. En esta lección puedes conseguir ese cambio con unas pocas propiedades.

**Acción:** mostrar la portada dentro del mismo intervalo y alternar una vez entre la tarjeta inicial y la resuelta.

### 00:35–00:55 Color y fondo

**Narración**

`color` cambia el color del texto. `background-color` cambia el fondo. Piensa en una hoja y un lápiz: una cosa es el color de la hoja y otra, el de las letras. Conviene elegir colores que permitan leer con facilidad.

**Acción:** señalar las dos propiedades de la diapositiva.

### 00:55–01:40 Demostración de colores

**Narración**

El ejemplo ya está escrito. En `body`, que representa el contenido de la página, aparece un fondo azul muy claro. En `p`, que corresponde a los párrafos, aparece un color oscuro. Observa lo que pasa al cambiar el fondo por blanco. El texto no cambia. Al restaurar el azul claro, vuelve el fondo anterior. Cada propiedad modifica una parte diferente de la apariencia.

**Acción:** en la solución, cambiar temporalmente `background-color: #eef4ff` por `white` y restaurarlo. Señalar `p { color: #25364c; }` y su resultado. No explicar códigos hexadecimales en detalle: son formas de indicar colores.

### 01:40–02:05 Fuente y tamaño

**Narración**

La fuente es la forma de las letras. `font-family` permite elegirla y `font-size` controla su tamaño. Un texto puede verse bonito y aun así ser difícil de leer si sus letras son demasiado pequeñas. La lectura debe resultar cómoda.

**Acción:** mostrar el concepto y regresar al editor.

### 02:05–02:45 Demostración de texto

**Narración**

Aquí aparece Arial como fuente. El párrafo tiene un tamaño de dieciocho píxeles. Si el tamaño baja a doce, el texto resulta más pequeño; al volver a dieciocho, recupera su tamaño. `line-height` deja espacio entre las líneas. No cambia lo que dice el párrafo: ayuda a que las líneas no queden demasiado juntas.

**Acción:** cambiar `font-size` de `18px` a `12px` y restaurarlo. Señalar `line-height: 1.5` sin abrir una explicación de unidades o herencia.

### 02:45–03:15 Espacios y borde

**Narración**

El borde marca el contorno de la tarjeta. `padding` deja espacio dentro, entre el texto y el borde. `margin` deja espacio fuera y la separa de lo que tiene alrededor. Una forma de recordarlo es pensar en una caja: el relleno está dentro y la separación con otras cajas está fuera.

**Acción:** señalar el contenido, el espacio interior y el exterior en la diapositiva. Evitar explicar todas las variantes de cada propiedad.

### 03:15–04:10 Demostración de tarjeta

**Narración**

Este bloque ya tiene el nombre `card`. Sus reglas forman la tarjeta. Con `padding: 24px`, el texto deja de estar pegado al borde. Con `border` aparece una línea alrededor. `border-radius` redondea las esquinas. El margen deja espacio por fuera; en este ejemplo también permite centrar la tarjeta. Observa cada cambio por separado para identificar qué propiedad lo produce.

**Acción:** señalar las cuatro reglas en el código preparado. Cambiar `padding` a `0`, observar el texto junto al borde y restaurar `24px`. Mostrar brevemente el borde y las esquinas. No escribir la tarjeta desde cero.

### 04:10–05:50 Pruebas y comparación

**Narración**

Ahora compara tres detalles. Primero, el tamaño del texto: debe leerse sin acercarse demasiado a la pantalla. Después, el espacio interior: el contenido necesita separarse del borde. Por último, los colores: un texto oscuro sobre un fondo claro se distingue mejor que dos colores muy parecidos. También puedes alinear el título al centro con `text-align`. Cambia una propiedad a la vez y comprueba el resultado antes de continuar. Así resulta más fácil reconocer qué hizo cada cambio.

**Acción:** realizar tres comparaciones breves: `font-size: 18px` frente a `12px`; `padding: 24px` frente a `0`; color oscuro frente a uno demasiado claro. Restaurar los valores de la solución. Mostrar `text-align: center` en el título. Este tramo reserva tiempo para observar los resultados, no para añadir propiedades nuevas. Si la grabación va retrasada, reducir las repeticiones y pasar al reto.

### 05:50–06:40 Reto

**Narración**

Ahora puedes personalizar tu tarjeta. El HTML ya está preparado: no necesitas empezar desde cero. Cambia el fondo y elige una fuente. Después, agrega un borde y espacio interior con `padding`. Comprueba que el texto se lea bien. Como desafío adicional, separa la tarjeta con `margin` y redondea sus esquinas. Pausa el video para completar la actividad y compara tu resultado con la solución cuando termines. Tu tarjeta puede tener otros colores y seguir siendo correcta.

**Acción:** mostrar la actividad inicial y señalar sus comentarios. No resolver el ejercicio en el video ni esperar a que el estudiante lo termine.

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
