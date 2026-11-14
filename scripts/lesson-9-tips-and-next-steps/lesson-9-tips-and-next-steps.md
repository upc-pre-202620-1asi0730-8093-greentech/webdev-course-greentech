# Lección 9 Consejos y próximos pasos

- **Duración máxima del video:** 5 minutos.
- **Objetivo de grabación:** entre 4:40 y 4:50; nunca superar 5:00.
- **Público:** estudiantes de secundaria que completaron las lecciones anteriores.
- **Resultado:** reconocer errores sencillos y revisar una página antes de compartirla.

## Materiales

- [Presentación](lesson-9-tips-and-next-steps-presentation.pptx).
- [HTML inicial con errores preparados](../../starter-files/lesson-9-tips-and-next-steps/index.html) y [CSS inicial](../../starter-files/lesson-9-tips-and-next-steps/styles.css).
- [HTML corregido](../../completed-examples/lesson-9-tips-and-next-steps/index.html) y [CSS corregido](../../completed-examples/lesson-9-tips-and-next-steps/styles.css).
- Comparación de formato: [una sola línea](../../starter-files/lesson-9-tips-and-next-steps/formatting-example.html) y [código ordenado](../../completed-examples/lesson-9-tips-and-next-steps/formatting-example.html).

## Preparación antes de grabar

Usar el mismo editor en el navegador que en las lecciones previas. Preparar una pestaña con el ejemplo inicial y otra con la solución, además de los dos ejemplos de formato. Si el editor separa los paneles HTML y CSS, pegar cada contenido en su panel y retirar el enlace a `styles.css` de la copia del HTML si el editor enlaza los estilos automáticamente.

El archivo inicial contiene errores intencionales y no representa una solución correcta: el título abre con `<h1>` y cierra incorrectamente con `</h2>`, falta `:` en una declaración CSS, el texto de los párrafos es demasiado claro y la imagen no tiene `alt`. Las correcciones se detallan en cada tramo del guion. El ejemplo separado de formato sí es válido y permite comparar sangría sin mezclarla con la corrección de errores.

La imagen de ejemplo requiere conexión a Internet. Comprobar antes de grabar que carga la URL utilizada por el HTML. Su texto alternativo esperado es «Cartel con el texto Club de lectura». No pedir fotografías ni datos personales al estudiante.

## Cronograma de referencia

| Intervalo máximo | Contenido | Qué se muestra |
| --- | --- | --- |
| 00:00–00:25 | Introducción | Portada. |
| 00:25–00:50 | Orden del código | Concepto de sangría y nombres claros. |
| 00:50–01:25 | Comparación de formato | Dos archivos preparados en el editor. |
| 01:25–01:50 | Errores frecuentes | Cierre HTML y dos puntos en CSS. |
| 01:50–02:35 | Corrección | Editor y resultado. |
| 02:35–03:00 | Lectura y texto alternativo | Diapositiva de accesibilidad. |
| 03:00–03:45 | Mejora de la página | Comparar contraste y agregar `alt`. |
| 03:45–04:10 | Próximos pasos | Ideas pequeñas y documentación. |
| 04:10–04:45 | Reto independiente | Lista de revisión. |
| 04:45–05:00 | Despedida | Cierre; detener antes de 5:00. |

Los cambios de ventana y la portada forman parte de estos tiempos. Las diapositivas que indican «cambiar al editor» son guías del presentador; en el video se muestra el editor real.

## Guion para la grabación

### 00:00–00:25 Introducción

**Narración**

Antes de compartir tu página, conviene revisar algunos detalles. En esta lección puedes ordenar el código, corregir errores sencillos y comprobar que el contenido se lea con facilidad. El objetivo es mejorar lo que ya existe.

**Acción:** mostrar la portada y la página preparada, sin resolver todavía los errores.

### 00:25–00:50 Orden del código

**Narración**

Un código ordenado se parece a un cuaderno con sus ideas separadas. Los espacios al comienzo de cada línea ayudan a reconocer qué elementos están dentro de otros. Esos espacios se llaman sangría. También conviene usar nombres que permitan reconocer para qué sirve cada parte.

**Acción:** mostrar el concepto. No añadir reglas avanzadas de formato.

### 00:50–01:25 Comparación de formato

**Narración**

Observa estas dos versiones. La primera está escrita en una sola línea; la segunda separa las etiquetas y deja espacios al comienzo. Las dos muestran la misma página. La diferencia está en lo fácil que resulta leer el código. En la segunda puedes encontrar el título y el párrafo con mayor rapidez.

**Acciones para grabar:** abrir el archivo inicial `formatting-example.html` en una pestaña separada del ejercicio principal. Mostrar su única línea y localizar «Club de lectura». Mostrar después la versión ordenada del mismo archivo en completed-examples. Señalar las líneas de `main`, `h1` y `p` y los espacios al comienzo. Ejecutar ambas: tienen el mismo título y párrafo. Este ejemplo solo explica el orden; no reemplazar con él el HTML principal, que también contiene la imagen y un segundo párrafo. Regresar al ejercicio principal al terminar.

### 01:25–01:50 Errores frecuentes

**Narración**

Al escribir es normal olvidar un detalle. Una etiqueta puede cerrarse con un nombre distinto, y una propiedad de CSS puede perder los dos puntos que separan su nombre del valor. Si algo no aparece como esperabas, revisa primero esas partes. Cambia un detalle y comprueba el resultado.

**Acción:** señalar el cierre incorrecto y `color #2458e8;` en el ejemplo inicial.

### 01:50–02:35 Corrección en pantalla

**Narración**

El título empieza con hache uno, pero termina con hache dos. El inicio y el cierre deben coincidir. Al corregirlo, la estructura queda bien escrita. Es posible que el navegador ya mostrara el título correctamente: a veces intenta acomodar estos errores. Ahora falta un signo en CSS. Al agregar los dos puntos después de color, el título recibe su color azul.

**Acciones para grabar:**

1. Regresar al HTML principal `index.html`, no al ejemplo de formato.
2. Localizar `<h1>Club de lectura</h2>`. Cambiar únicamente `</h2>` por `</h1>`.
3. Ejecutar. Si no hay diferencia visible, explicar lo indicado en la narración; no afirmar que cambió el tamaño o la posición.
4. Abrir `styles.css`, localizar `h1` y cambiar `color #2458e8;` por `color: #2458e8;`.
5. Ejecutar y señalar el título azul. Mantener las dos correcciones.

### 02:35–03:00 Lectura y texto alternativo

**Narración**

Si el texto tiene un color parecido al fondo, cuesta leerlo. Las imágenes que comunican información necesitan una descripción breve con `alt`. Esa descripción ayuda si la imagen no carga o una herramienta lee la página en voz alta.

**Acción:** mostrar el concepto. No afirmar que todas las imágenes deben tener una descripción larga: las imágenes decorativas pueden usar `alt=""`.

### 03:00–03:45 Mejora de la página

**Narración**

Aquí los párrafos casi se pierden sobre el fondo blanco. Al elegir un color oscuro, se distinguen mejor. La imagen muestra un cartel del club de lectura, así que su descripción debe comunicar eso. `alt` no es un título visible debajo de la imagen: es una alternativa para comprender su contenido. La descripción debe ser útil y corresponder a lo que aparece.

**Acciones para grabar:**

1. En el CSS principal, localizar `p` y sustituir `color: #e8edf5;` por `color: #25364c;`. Ejecutar y señalar los dos párrafos, ahora oscuros sobre blanco.
2. Regresar al HTML principal. Localizar la única etiqueta `img`; conservar completa la dirección de `src`.
3. Antes de su `>`, añadir un espacio y `alt="Cartel con el texto Club de lectura"`. Ejecutar.
4. Señalar el atributo en el código. La imagen debe seguir apareciendo igual: `alt` no agrega un pie de foto visible. No cambiar ni borrar la dirección para simular un fallo durante esta toma.
5. Comparar con la solución únicamente al finalizar: deben conservarse el título, los dos párrafos y la misma imagen.

### 03:45–04:10 Próximos pasos

**Narración**

Puedes seguir practicando con una tarjeta de pasatiempos, una pequeña galería o una página sobre un club escolar. Elige un cambio por vez. Si necesitas recordar una etiqueta o propiedad, MDN Web Docs ofrece ejemplos y explicaciones en español. No es necesario memorizar todo para continuar aprendiendo.

**Acción:** mostrar las ideas y el enlace de referencia, sin navegar por documentación durante el video.

### 04:10–04:45 Reto final

**Narración**

Ahora revisa la página de esta actividad o tu proyecto anterior. Primero, comprueba que las etiquetas estén cerradas. Después, corrige una propiedad CSS y elige colores que permitan leer el texto. Por último, revisa la descripción de una imagen que comunique información. Pausa el video para hacerlo y compara tu trabajo con la solución cuando termines.

**Acción:** señalar los tres pasos de la diapositiva. No resolver otro proyecto completo ni esperar durante la grabación.

### 04:45–05:00 Despedida

**Narración**

Ya tienes una lista para revisar tus páginas. Sigue practicando con proyectos pequeños y mejora un detalle cada vez.

**Acción:** mostrar el cierre y detener la grabación, sin añadir otra recapitulación.

## Criterios del reto

- El título termina antes del párrafo y el HTML conserva su estructura.
- La propiedad `color` tiene dos puntos y un valor válido.
- Los párrafos se distinguen del fondo.
- La imagen informativa tiene una descripción breve y pertinente.

La solución es una referencia, no un diseño obligatorio. No se necesitan JavaScript, instalaciones ni cuentas adicionales para comprender el ejercicio.

## Control de duración

Ensayar con cronómetro incluyendo los cambios de ventana y las cuatro correcciones. Si la grabación va retrasada, reducir las comparaciones y evitar abrir páginas externas. Los tiempos de lectura son orientativos: solo el ensayo permite comprobar la duración real. Mantener la actividad como tarea con el video pausado y terminar antes del límite de cinco minutos.

## Referencia para continuar

[Aprender desarrollo web en MDN](https://developer.mozilla.org/es/docs/Learn_web_development).

## Hoja de control para grabar

Leer únicamente la **Narración**. Las acciones indican qué hacer con el cursor y no se leen al estudiante. Los intervalos incluyen la escritura y el tiempo para observar el resultado; no agregar la lectura de estas instrucciones al video.

Antes de grabar en Windows:

1. Preparar el editor del navegador con `index.html` y `styles.css` de starter-files de esta lección. Ejecutar y comprobar que aparece la imagen. Los párrafos serán demasiado claros y el título no tendrá aplicado su azul: son errores preparados.
2. Preparar aparte las dos versiones de `formatting-example.html`. No mezclar esos archivos con la tarjeta principal: tienen menos contenido porque solo ilustran la sangría.
3. Dejar la solución principal como referencia, sin pegarla durante la explicación. Abrir la presentación y ensayar con cronómetro antes de grabar.
4. Mostrar la presentación en los tramos conceptuales y el editor en las demostraciones. Las diapositivas ocultas son instrucciones del presentador. Sus fragmentos breves ilustran la idea; en el editor se usa el archivo real Club de lectura y su dirección de imagen, sin reemplazarla por imagen.png.
5. Tras el ensayo, recargar los archivos iniciales. Grabar una toma con los cuatro cambios, respetando el límite de cinco minutos.

| Momento | Archivo de trabajo | Cambio permanente | Comprobación |
| --- | --- | --- | --- |
| 01:50–02:35 | index.html | Cierre h2 por cierre h1 | El título abre y cierra con el mismo nombre. |
| 01:50–02:35 | styles.css | Agregar : después de color en h1 | Título azul. |
| 03:00–03:45 | styles.css | Color de p a #25364c | Ambos párrafos legibles. |
| 03:00–03:45 | index.html | Añadir alt a img | Descripción presente en código; misma imagen visible. |

Las cuatro correcciones llevan de los archivos iniciales a los resueltos sin cambiar el contenido ni el diseño de la tarjeta. El ejemplo de sangría se compara por separado y no forma parte de esas cuatro correcciones. Para practicar el reto, el estudiante puede abrir otra copia inicial; no se deshace el trabajo de la demostración.

**Si el tiempo se agota:** reducir el recorrido del cursor y las repeticiones. No omitir las cuatro correcciones ni acelerar la voz. No abrir documentación externa ni resolver el reto durante la toma. Si la imagen no carga, comprobar la conexión antes de grabar; no sustituirla sin adaptar también su descripción.
