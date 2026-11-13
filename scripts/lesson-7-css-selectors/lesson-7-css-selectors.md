# Lección 7: Selectores CSS

**Enlace**: [Ver la lección]()

## ¿Qué son los selectores?

Los selectores en CSS son indicadores que sirven para elegir a un grupo de elementos a los cuales se les aplicará un estilo. Suelen seguir la forma:

`(Selector)` `{` `(Estilos)` `}`

Pueden combinarse varios selectores y aplicarles un mismo estilo. Se separan por una coma:

`(Selector)`, `(Selector)`, `(Selector)` `{` `(Estilos)` `}`

### Selectores por etiqueta HTML

Aplica un estilo a todas las etiquetas elegidas.

El siguiente selector aplica un color a todos los párrafos del documento HTML:

```css
p { color: #25364c;}
```

El siguiente selector aplica un color de fondo al cuerpo del documento HTML:

```css
body { background-color: #eef4ff; }
```

### Selectores por clase

Las clases son un atributo en HTML que permite identificar y agrupar a varios elementos. 

```html
<p class="resaltado grande"> Un parrafo resaltado </p>
```

Un elemento puede tener varias clases separadas entre sí por espacios.

```html
<p class="resaltado grande"> Un parrafo resaltado y con letra grande </p>
```

Con CSS se le puede aplicar un mismo estilo a todos los elementos que tengan la misma clase.

Por ejemplo, se tiene al siguiente estilo, usa `.` para elegir a los elementos de la clase 'resaltado' y cambia su color de fondo a uno amarillo:

```css
.resaltado { background-color: #FFFF00; }
```

A los siguientes elementos se le aplicará el estilo porque el nombre de la clase coincide con la definida en el CSS:

```html
<p class="resaltado"> Parrafo resaltado </p>
<p class="resaltado grande"> Otro parrafo resaltado </p>
```

A los siguientes elementos no se les aplicará el estilo porque no contienen la clase o no coincide su nombre:

```html
<p class="Resaltado"> Parrafo normal </p>
<p> Otro parrafo normal </p>
```

### Selectores por identificador

Los identificadores son un atributo en HTML que permite identificar a un solo elemento en el documento. Al igual que con las clases, se le puede seleccionar y aplicar estilos con CSS, pero no se recomienda que se aplique a varios elementos.

Se tiene el siguiente estilo, usa `#` para elegir un identificador y alinea todo el texto al centro:

```css
#seccion-b { text-align: center; }
```

Se aplicará el estilo al siguiente elemento, pues el identificador coincide:

```html
<h2 id="seccion-b"> Seccion B </h2>
```

No se aplicará el estilo al siguiente elemento porque no tiene el identificador seleccionado:

```html
<h2 id="seccion-a"> Seccion A </h2>
```

### Selector universal

Este selector aplica un mismo estilo a todos los elementos HTML de la página sin importar su etiqueta, clase o identificador. Se representa por un asterisco `*`.

El siguiente estilo cambia la tipografía de todos los textos a Arial:

```css
* { font-family: Arial; }
```

Todos los elementos son afectados:

```html
<h1> Titulo </h1>
<p class="parrafo"> Primer parrafo </p> 
<button id="accion"> Boton </button>
```