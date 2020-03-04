# 1. Introducción 01:29:38

## Bienvenida 03:11

En un proyecto de desarrollo Web nos podemos encontrar 4 etapas fundamentales:

1. Etapa del Diseño y la Planeación
2. Etapa de la Arquitectura de ese Diseño (Desarrollador Front End)
3. Etapa de Interacción del Diseño (Desarrollador Back End)
4. Etapa de Entrega y Pruebas.

Este curso cubre solo la etapa 2.

## Material de apoyo e inquietudes 05:18

Contiene todo el código fuente de los proyectos, cada sección tiene su código.

## Contáctame 00:12

Siempre me encanta conectarme con mis alumnos, incluso para saludar :)

Tengo una página personal, otra de de Facebook, una cuenta de Twitter, una cuenta de LinkedIn y un canal de Youtube.

Encontrará información útil de forma gratuita, descuentos para los cursos y también será mucho más fácil mantenerse actualizado sobre mis proyectos:

https://www.udemy.com/user/juanunativa/

Juan Fernando Urrego

Diseñador Visual y Desarrollador Web

## Editor de código y plugins 16:30

El instructor trabaja con [Sublime Text](https://www.sublimetext.com/)

Descargar e Intsalar el [Package Controll](https://packagecontrol.io/)

 Plugins:
 
* Emmet
* AdvancedNewFile
* AutoFileName
* Bootstrap 4 Autocomplete
* BrackeHighlighter
* Comment-Snippets
* Console Wrap
* HTML Minifier
* JsFormat-master

## ¿Qués es el desarrollo Front-End? 08:31

El término FRONT-END también conocido como lado del cliente, es la parte del sitio web con la que interactúa el usuario final.

Buena experiencia de usuario, inmersión y usabilidad son alguno de los objetivos que busca un buen FRONT-END.

Lenguajes del Front End

1. HTML
2. CSS
3. JS

## Fundamentos de HTML5 13:32

Estructura básica de HTML.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

Algunas etiquetas que se usan en HTML son:

```html
<div></div>

<header></header>

<nav></nav>

<section></section>

<article></article>

<footer></footer>

<video src=""></video>

<audio src=""></audio>
```

## Fundamentos de CSS3 12:03

Nos permite dar estilo a nuestro sitio Web.

Archivo con extensión `.css`

Para llamar un archivo CSS desde HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="style.css">
</head>
<body>
```

`style.css`:

```css
/*Reglas CSS*/

#myId{
   padding: 30px;
   background: red;
   color: yellow;
}

.myClass{
   padding: 20px;
   background: blue;
   color: white;
}

div{
   padding: 10px;
   background: white;
   color: white;
}

div#myId{
   padding: 30px;
   background: red;
   color: yellow;
}

div.myClass{
   padding: 20px;
   background: blue;
   color: white;
}

```

## Fundamentos de Javascript 18:08

JS permite hacer dinámico nuestro sitio Web. 

Archivo con extensión `.js`

Para llamar un archivo JS desde HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <script src="script.js"></script>
</head>
<body>
```

`script.js`

```js
// Variables
/*
texto
numeros
booleans
arrays
objectos
*/

//Condiciones

// Funciones

// Eventos

```

## Fundamentos de jQuery 12:13

[JQuery](https://jquery.com/) optimiza el código JS

Para llamar usar JQuery CDN desde HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/jquerymobile/1.4.5/jquery.mobile.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquerymobile/1.4.5/jquery.mobile.min.js"></script>
</head>
<body>
</body>
</html>
```



