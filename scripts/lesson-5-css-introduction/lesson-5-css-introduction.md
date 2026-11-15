# Lección 5: Introducción a CSS

**Enlace**: [Ver la lección](https://youtu.be/-u37OClg4YI?si=5NDpbfziCC5rt2tQ)

## Preparación

Antes de comenzar, coloca `index.html` y `styles.css` en la misma carpeta. El archivo HTML ya contiene una página personal sencilla y está conectado con la hoja de estilos mediante la etiqueta `<link>`.

Durante la demostración se agregan las reglas CSS poco a poco. La presentación sirve como guía, pero las demostraciones deben realizarse en el editor con el código preparado.

## ¿Qué es CSS?

HTML organiza el contenido de una página web. CSS, que significa *Cascading Style Sheets*, permite controlar cómo se muestran visualmente esos elementos.

Con CSS podemos cambiar:

- El color del texto y del fondo.
- El tipo y el tamaño de la fuente.
- El espacio interior y exterior.
- Los bordes y las esquinas de una tarjeta.
- La alineación del texto.

Una página creada solamente con HTML puede funcionar correctamente, pero CSS ayuda a mejorar su apariencia y legibilidad.

## Reglas CSS

Una regla CSS contiene un selector y una o más declaraciones. El selector identifica el elemento que queremos modificar. Cada declaración combina una propiedad con un valor.

```css
h1 {
  color: #2458E8;
}
```

En este ejemplo:

- `h1` es el selector.
- `color` es la propiedad.
- `#2458E8` es el valor.

Las declaraciones se escriben entre llaves y terminan con punto y coma.

## Conectar HTML y CSS

La etiqueta `<link>` dentro de `<head>` conecta el documento HTML con el archivo CSS:

```html
<link rel="stylesheet" href="styles.css">
```

El contenido de la página se escribe en `index.html` y las reglas de presentación se escriben en `styles.css`.

## Color del título

El siguiente HTML contiene un título dentro de una tarjeta:

```html
<main class="tarjeta">
  <h1>Mi perfil</h1>
  <p>Este es mi primer ejemplo con CSS.</p>
</main>
```

Podemos cambiar el color del título utilizando el selector `h1`:

```css
h1 {
  color: #2458E8;
}
```

El selector apunta a los elementos `<h1>` y la propiedad `color` cambia el color de sus letras.

## Fondo y fuente

El selector `body` permite aplicar estilos al contenido general de la página:

```css
body {
  background-color: #eaf4ff;
  font-family: Arial, sans-serif;
}
```

`background-color` cambia el color del fondo. `font-family` permite elegir el tipo de letra. `Arial, sans-serif` indica que se debe usar Arial y, si no está disponible, otra fuente sin serifas.

## Selectores de clase

En HTML podemos asignar una clase con el atributo `class`:

```html
<main class="tarjeta">
  <h1>Mi perfil</h1>
  <p>Este es mi primer ejemplo con CSS.</p>
</main>
```

En CSS escribimos un punto seguido del nombre de la clase:

```css
.tarjeta {
  background-color: white;
  padding: 24px;
  border: 2px solid #2458E8;
  border-radius: 12px;
}
```

Esta regla se aplica al elemento que tiene `class="tarjeta"`.

- `background-color` establece el fondo blanco.
- `padding` crea espacio entre el contenido y el borde.
- `border` agrega un borde azul de dos píxeles.
- `border-radius` redondea las esquinas.

## Alinear el texto

La propiedad `text-align` controla la alineación del texto. Para centrar el título utilizamos el valor `center`:

```css
h1 {
  color: #2458E8;
  text-align: center;
}
```

Si cambiamos `center` por `left`, el título vuelve a alinearse a la izquierda. Podemos probar ambos valores en la vista previa y dejar `center` como resultado final.

## Código completo

### index.html

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi perfil</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <main class="tarjeta">
    <h1>Mi perfil</h1>
    <p>Este es mi primer ejemplo con CSS.</p>
  </main>
</body>
</html>
```

### styles.css

```css
h1 {
  color: #2458E8;
  text-align: center;
}

body {
  background-color: #eaf4ff;
  font-family: Arial, sans-serif;
}

.tarjeta {
  background-color: white;
  padding: 24px;
  border: 2px solid #2458E8;
  border-radius: 12px;
}
```

En la vista previa, el título aparece azul y centrado, el fondo de la página es azul claro y el contenido está dentro de una tarjeta blanca con borde y esquinas redondeadas.

## Comparación con y sin CSS

Si comentamos temporalmente la etiqueta `<link>`, el navegador continúa mostrando el título y el párrafo, pero utiliza sus estilos predeterminados:

```html
<!-- <link rel="stylesheet" href="styles.css"> -->
```

Al quitar el comentario, la página vuelve a cargar los estilos de `styles.css`. El contenido HTML sigue siendo el mismo; CSS modifica su presentación.

## Ejercicio

Personaliza la página del ejercicio utilizando `index.html` y `styles.css`:

- Usa `body` para cambiar el fondo y elegir una fuente.
- Usa `.tarjeta` para agregar fondo blanco, borde y espacio interior.
- Usa `h1` para cambiar el color del título y centrarlo con `text-align`.
- Comprueba que `index.html` esté conectado a `styles.css`.

Puedes elegir otros colores y valores siempre que el texto se lea con claridad.

**Práctica**: [Clic para programar](https://onecompiler.com/html/45993vpws)

**Solución**: [Ver archivos resueltos](https://onecompiler.com/html/459944jda)

## Cierre

En esta lección aprendimos a conectar HTML con CSS, crear reglas, utilizar selectores y cambiar colores, fuentes, espacios, bordes y alineación. Continúa practicando y observa cómo cada propiedad modifica la apariencia de la página.
