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

El archivo inicial contiene errores intencionales y no representa una solución correcta: falta `</h1>`, falta `:` en una declaración CSS, el texto de los párrafos es demasiado claro y la imagen no tiene `alt`. Los comentarios indican dónde intervenir. El ejemplo separado de formato sí es válido y permite comparar sangría sin mezclarla con la corrección de errores.

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

**Acción:** alternar entre los dos archivos `formatting-example.html`. No modificar contenido ni afirmar que la sangría cambia la apariencia de la página.

### 01:25–01:50 Errores frecuentes

**Narración**

Al escribir es normal olvidar un detalle. Una etiqueta puede quedar sin cerrar, y una propiedad de CSS puede perder los dos puntos que separan su nombre del valor. Si algo no aparece como esperabas, revisa primero esas partes. Cambia un detalle y comprueba el resultado.

**Acción:** señalar el cierre ausente y `color #2458e8;` en el ejemplo inicial.

### 01:50–02:35 Corrección en pantalla

**Narración**

Este título necesita terminar antes de que empiece el párrafo. Al agregar `</h1>`, queda separado correctamente. En CSS falta un signo después de `color`. La forma correcta es `color:`, seguido del color elegido y un punto y coma. Al corregirlo, el título recibe su color azul. Un error pequeño puede impedir que se aplique un estilo.

**Acción:** agregar `</h1>` en el HTML y `:` en el CSS. Comprobar el título y el párrafo. No añadir más errores durante la demostración. Si el navegador ya había acomodado parte del HTML, aclarar brevemente que verlo bien no significa que esté bien escrito.

### 02:35–03:00 Lectura y texto alternativo

**Narración**

Si el texto tiene un color parecido al fondo, cuesta leerlo. Las imágenes que comunican información necesitan una descripción breve con `alt`. Esa descripción ayuda si la imagen no carga o una herramienta lee la página en voz alta.

**Acción:** mostrar el concepto. No afirmar que todas las imágenes deben tener una descripción larga: las imágenes decorativas pueden usar `alt=""`.

### 03:00–03:45 Mejora de la página

**Narración**

Aquí los párrafos casi se pierden sobre el fondo blanco. Al elegir un color oscuro, se distinguen mejor. La imagen muestra un cartel del club de lectura, así que su descripción debe comunicar eso. `alt` no es un título visible debajo de la imagen: es una alternativa para comprender su contenido. La descripción debe ser útil y corresponder a lo que aparece.

**Acción:** cambiar el color de `p` a `#25364c` y añadir `alt="Cartel con el texto Club de lectura"`. Señalar el atributo sin prometer que aparezca como un pie de foto. El fondo y la tarjeta ya están preparados.

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
