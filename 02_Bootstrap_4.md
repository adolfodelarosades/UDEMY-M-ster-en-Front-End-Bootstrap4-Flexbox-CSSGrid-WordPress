# 2. Bootstrap 4 01:13:49

Referencias

https://getbootstrap.com/

https://www.w3schools.com/bootstrap4/

http://bootstrap4.guide/

https://w3layouts.com/


## ¿Qué es Bootstrap? 07:20

* Bootstrap es un marco de trabajo o framework de libre uso para hacer del desarrollo web algo más rápido y más fácil.
* Bootstrap incluye plantillas de diseño basadas en HTML y CSS con tipografías, formas, botones, tablas de navegación modales, carruseles de imágenes y muchos otros elementos, así como complementos opcionales de JS.
* Bootstrap también da la posibilidad de crear fácilmente diseños que responden a cualquier pantalla o dispositivo.

<img src="images/c2/2-responsivo.png">

<img src="images/c2/2-b3-b4.png">

## Instalación de Bootstrap 4 11:26

<img src="images/c2/2-intalar.png">

### 1. Usando CDN

Insertamos el código MaxCDN ([página](https://www.w3schools.com/bootstrap4/bootstrap_get_started.asp)) dentro del header.

`index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>

    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css">

    <!-- jQuery library -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

    <!-- Popper JS -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>

    <!-- Latest compiled JavaScript -->
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js"></script>
</head>
<body>
    
</body>
</html>
```

### 2. Forma Local

Para instalar localmente Bootstrapt tengo que crearme una estructura como la siguiente e copiar los archivos CSS y JS a la carpeta correspondiente.

<img src="images/c2/2-estructura.png">

Y en mi archivo HTML hacer el llamado a mis archivos locales:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>

    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="css/bootstrap.min.css">

    <!-- jQuery library -->
    <script src="js/jquery.min.js"></script>

    <!-- Popper JS -->
    <script src="js/popper.min.js"></script>

    <!-- Latest compiled JavaScript -->
    <script src="js/bootstrap.min.js"></script>
</head>
<body>
    
</body>
</html>
```

<img src="images/c2/2-referencias.png">

[Referencias](https://www.w3schools.com/bootstrap4/bootstrap_ref_all_classes.asp)

## Sistema de Grids (Rejillas) 19:05

[Grid System](https://www.w3schools.com/bootstrap4/bootstrap_grid_basic.asp)

<img src="images/c2/2-rejilla.png">

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```
[Código tomado de 2. **Bootstrap 4 is mobile-first**](https://www.w3schools.com/bootstrap4/bootstrap_get_started.asp)

Este código va dentro de la HEAD.

<img src="images/c2/2-resolucion.png">

En el sistema de Grids o Rejillas Bootstrap usa un máximo de 12 columnas.

Independiente del tamaño de pantalla nosotros trabajaremos con columnas.

<img src="images/c2/2-grids.png">

Me puedo auxiliar de las herramientas de desarrollador para ver el Diseño Responsive y cambiar a los tamaños de resoluciones permitidos.

* Full HD - HD: 1920px
* Portatil: 1366px
* Tablet Horizontal: 1024px
* Tablet Vertical 768px
* Móvil Horizontal: 576px
* Móvil Vertical: 320px

<img src="images/c2/2-responsive.png">

**En cualquiera de estos 12 tamaños puedo tener hasta 12 columnas**

<img src="images/c2/2-col-1.png">

<img src="images/c2/2-col-2.png">

[Grid Options](https://www.w3schools.com/bootstrap4/bootstrap_grid_system.asp)

### Trabajar con Sistemas de Grids de Bootstrap

Lo primero que debemos definir en un sistema Grid de Bootstrap es un **Contenedor** y tenemos dos tipos:

* **`container`**
* **`container-fluid`**

Si usamos `container` tendremos **tamaños fijos para el contenedor según el tamaño del dispositivo** que estemos usando, como podemos ver en la siguiente tabla:

<img src="images/c2/2-container.png">

Si en lugar de usar `container` usamos `container-fluid` el contenedor usara todo el ancho de la página independientemente del dispositivo que usemos.

```html
<body> 
    <div class="container-fluid">

    </div>
</body>
```

Dentro del contenedor tendremos filas o renglones las cuales definimos con la clase `row`:

```html
<body> 
    <div class="container-fluid">
        <div class="row">

        </div>
    </div>
</body>
```

Dentro de la fila creamos nuestras columnas con la diferentes clases que tenemos:

* `col-N`
* `col-sm-N`
* `col-md-N`
* `col-lg-N`
* `col-xl-N`

**N**: Número del 1-12

```html
<body> 
    <div class="container-fluid">
        <div class="row">
            <div class="col-12">Col 12</div>
            <div class="col-6">Col 6</div>
            <div class="col-6">Col 6</div>
        </div>
    </div>
</body>
```

Veamos el siguiente código y su salida:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>

    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="css/bootstrap.min.css">

    <!-- jQuery library -->
    <script src="js/jquery.min.js"></script>

    <!-- Popper JS -->
    <script src="js/popper.min.js"></script>

    <!-- Latest compiled JavaScript -->
    <script src="js/bootstrap.min.js"></script>
</head>
<body> 
    <div class="container-fluid">
        <div class="row">
            <div class="col-12 bg-danger">Col 12</div>
            
            <div class="col-6 bg-primary">Col 6</div>
            <div class="col-6 bg-secondary">Col 6</div>
            
            <div class="col-4 bg-success">Col 4</div>
            <div class="col-4 bg-warning">Col 4</div>
            <div class="col-4 bg-info">Col 4</div>
            
            <div class="col-3 badge-danger">Col 3</div>
            <div class="col-3 bg-primary">Col 3</div>
            <div class="col-3 bg-secondary">Col 3</div>
            <div class="col-3 bg-success">Col 3</div>            
            
            <div class="col-2 bg-success">Col 2</div>
            <div class="col-2 badge-warning">Col 2</div>
            <div class="col-2 bg-info">Col 2</div>
            <div class="col-2 badge-danger">Col 2</div>
            <div class="col-2 bg-primary">Col 2</div>
            <div class="col-2 bg-secondary">Col 2</div>            
        </div>
    </div>
</body>
</html>
```

<img src="images/c2/2-columnas.png">

Si en lugar de `container-fluid` usamos `container` tenemos:

<img src="images/c2/2-columnas-2.png">

Tambien podemos ver la vista responsiva para cada uno de los tamaños de dispositivos:

<img src="images/c2/2-320.png">

<img src="images/c2/2-540.png">

<img src="images/c2/2-720.png">

<img src="images/c2/2-960.png">

<img src="images/c2/2-1140.png">

## Las Clases CSS de Bootstrap 4 - Parte 1 18:43

[Bootstrap 4 Class Reference](https://www.w3schools.com/bootstrap4/bootstrap_ref_all_classes.asp)


[¿Diseño web responsive o diseño web mobile first?](https://www.novvamarketing.com/blog-marketing-digital/diseno-web-responsive-o-diseno-web-mobile-first/)

Hay dos opciones de empezar el diseño:

* Responsive
* Mobile First

<img src="images/c2/2-diseno.png">

### Colores 

Los colores podemos verlos en [Bootstrap 4 Colors](https://www.w3schools.com/bootstrap4/bootstrap_colors.asp)

#### Text Colors

Las clases para el color de los textos son: 

`.text-muted`, `.text-primary`, `.text-success`, `.text-info`, `.text-warning`, `.text-danger`, `.text-secondary`, `.text-white`, `.text-dark`, `.text-body` (default body color/often black) and `.text-light`:

Ejemplo:

`textColor.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>

    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="css/bootstrap.min.css">

    <!-- jQuery library -->
    <script src="js/jquery.min.js"></script>

    <!-- Popper JS -->
    <script src="js/popper.min.js"></script>

    <!-- Latest compiled JavaScript -->
    <script src="js/bootstrap.min.js"></script>
</head>
<body> 
    <div class="container">
        <h2>Colores contextuales</h2>
        <p>Utilice las clases contextuales para proporcionar "significado a través de colores":</p>
        <p class="text-muted">Este texto está silenciado.</p>
        <p class="text-primary">Este texto es importante.</p>
        <p class="text-success">Este texto indica éxito.</p>
        <p class="text-info">Este texto representa alguna información.</p>
        <p class="text-warning">Este texto representa una advertencia.</p>
        <p class="text-danger">Este texto representa peligro.</p>
        <p class="text-secondary">Texto secundario.</p>
        <p class="text-dark">Texto gris oscuro.</p>
        <p class="text-body">Color de default del body (a menudo negro).</p>
        <p class="text-light">Este texto es gris claro (sobre fondo blanco)</p>
        <p class="text-white">Este texto es blanco (sobre fondo blanco)</p>
      </div>
</body>
</html>
```

<img src="images/c2/2-text-color.png">


## Las Clases CSS de Bootstrap 4 - Parte 2 13:50

## Diviértete con Bootstrap 4 03:25

## Aterrizando conceptos de Bootstrap 4 - 12 preguntas
