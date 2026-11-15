# Lección 4: Enlaces, imágenes y más

**Enlace**: [Ver la lección](https://youtu.be/Qek1f3ZVFag)

## Introducción

En las lecciones anteriores aprendimos a utilizar HTML para crear títulos, párrafos y organizar información. En esta lección agregaremos nuevos elementos para crear páginas más completas e interactivas:

- Enlaces hacia otros sitios web
- Imágenes
- Campos de texto para introducir información

Estos elementos se pueden combinar dentro de una misma página personal utilizando solamente HTML.

## Enlaces

La etiqueta `<a>` permite crear un enlace. El atributo `href` indica la dirección a la que accederá el navegador cuando el visitante haga clic.

```html
<a href="https://developer.mozilla.org/es/docs/Web/HTML">
  Aprender más sobre HTML
</a>
```

El texto escrito entre `<a>` y `</a>` es el que verá el visitante. El atributo `href` puede contener la dirección de otro documento o de otro sitio web.

Para abrir el enlace en una pestaña nueva se puede utilizar el atributo `target`. El atributo `rel` ayuda a mantener segura la relación con la página que se abrirá.

```html
<a
  href="https://developer.mozilla.org/es/docs/Web/HTML"
  target="_blank"
  rel="noopener noreferrer"
>
  Aprender más sobre HTML
</a>
```

## Imágenes

La etiqueta `<img>` permite mostrar una imagen en la página. El atributo `src` indica la dirección o ubicación del archivo de imagen y el atributo `alt` proporciona una descripción de su contenido.

```html
<img
  src="https://placehold.co/300x180/png"
  alt="Imagen de ejemplo para mi página personal"
>
```

El texto de `alt` es importante para la accesibilidad, ya que permite que las personas que utilizan lectores de pantalla conozcan qué representa la imagen. También se muestra cuando la imagen no puede cargarse.

La etiqueta `<img>` no necesita una etiqueta de cierre. Para usar una imagen externa se requiere conexión a Internet.

## Campos de texto

La etiqueta `<input>` crea un campo donde el visitante puede escribir información. El atributo `type="text"` indica que se trata de un campo de texto.

La etiqueta `<label>` muestra una descripción o pregunta asociada al campo. Sus atributos `for` e `id` deben tener el mismo valor para relacionar ambas etiquetas.

```html
<label for="hobby">¿Cuál es tu pasatiempo?</label>
<input id="hobby" type="text">
```

En este ejemplo, `for="hobby"` identifica el campo relacionado y `id="hobby"` identifica el elemento `<input>`. El visitante puede seleccionar el campo y escribir su respuesta.

También se puede agregar un texto de ayuda con el atributo `placeholder`:

```html
<input
  id="game"
  type="text"
  placeholder="Escribe tu videojuego favorito"
>
```

El texto del atributo `placeholder` desaparece cuando el visitante empieza a escribir.

## Integración de elementos

Los enlaces permiten navegar hacia otros recursos, las imágenes muestran contenido visual y los campos de texto permiten introducir información. A continuación se combinan estos elementos con un título y un párrafo dentro de una página personal.

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi página personal</title>
</head>
<body>
  <h1>Mi página personal</h1>
  <p>¡Hola! Bienvenido a mi sitio web.</p>

  <a
    href="https://developer.mozilla.org/es/docs/Web/HTML"
    target="_blank"
    rel="noopener noreferrer"
  >
    Aprender más sobre HTML
  </a>

  <img
    src="https://placehold.co/300x180/png"
    alt="Imagen de ejemplo para mi página personal"
  >

  <label for="hobby">¿Cuál es tu pasatiempo?</label>
  <input id="hobby" type="text">
</body>
</html>
```

Cada elemento cumple una función diferente:

- `<h1>` y `<p>` organizan la información.
- `<a>` permite navegar hacia otro recurso.
- `<img>` agrega contenido visual.
- `<label>` identifica un campo.
- `<input>` permite introducir datos.

## Comprobación

Para comprobar que la página funciona correctamente:

1. Haz clic en el enlace y verifica que se abra la dirección indicada.
2. Comprueba que la imagen se muestre debajo del enlace.
3. Selecciona el campo de texto y escribe un pasatiempo o un videojuego favorito.

## Ejercicio

Completa una página personal utilizando los elementos aprendidos:

- Agrega un enlace hacia un recurso donde puedas aprender más sobre HTML.
- Incorpora una imagen utilizando los atributos `src` y `alt`.
- Crea un campo de texto para que el visitante escriba su pasatiempo favorito.

Debes utilizar las etiquetas `<a>`, `<img>`, `<label>` e `<input>`. Recuerda que el atributo `alt` debe describir el contenido de la imagen y que los atributos `for` e `id` deben relacionar la pregunta con su campo.

**Práctica**: [Clic para programar](https://onecompiler.com/html/4598y4mss)

**Solución**: [Clic para ver](https://onecompiler.com/html/4598yvgc3)

## Cierre

En esta lección aprendimos a utilizar enlaces, imágenes y campos de texto para mejorar nuestras páginas HTML. En la siguiente lección aprenderemos a personalizarlas utilizando CSS.
