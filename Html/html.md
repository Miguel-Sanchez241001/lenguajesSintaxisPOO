# Sintaxis html

Ejemplos de html practicos y breves explicaciones.

## Contenido

- [Sintaxis html](#sintaxis-html)
  - [Contenido](#contenido)
  - [Estructura de documento](#estructura-de-documento)
    - [Contenido invisible](#contenido-invisible)
    - [Contenido visible](#contenido-visible)
  - [Sintaxis de una etiqueta](#sintaxis-de-una-etiqueta)
  - [Atributos Generales](#atributos-generales)
  - [Etiquetas mas Usadas](#etiquetas-mas-usadas)
  - [Elementos externos](#elementos-externos)
    - [Imagenes](#imagenes)
    - [Enlaces](#enlaces)
    - [Listas](#listas)
  - [Multimedia](#multimedia)
  - [Iframe](#iframe)
  - [Formularios](#formularios)
    - [Principales atributos](#principales-atributos)
      - [Modelo de form](#modelo-de-form)
    - [Input](#input)
      - [Atributos para input comunes](#atributos-para-input-comunes)
        - [**Ejemp**](#ejemp)
      - [Atributos para input poco comunes](#atributos-para-input-poco-comunes)
        - [**Ejemplo**](#ejemplo)
      - [Ejemplos de input poco vistos](#ejemplos-de-input-poco-vistos)
  - [Paginas recomendadas](#paginas-recomendadas)
  - [End](#end)
  
---

## Estructura de documento

- Archivos con extension .html o .htm.

```html
<!-- Este es un comentario-->
<!DOCTYPE html><!-- Declaracion de html5-->
<html> <!--Declaracion del documento-->
<head>   
    <!--Contenido invisible-->   
</head>
<body>
    <!-- Cuerpo del documento-->
</body>
</html>
```

[👆](#contenido)

---

### Contenido invisible

- link, metadatos, especificaciones SEO, especificaciones para navegadores
  
```html
<head>
 <meta charset="UTF-8">
 <meta http-equiv="X-UA-Compatible" content="IE=edge">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <link rel="stylesheet" href="">
 <title>Document</title>
</head>
```

[👆](#contenido)

---

### Contenido visible

- Cuerpo del documento, lo que el navegador mostrara.

```html
<body>
 <header>
    <nav>
        <ul>
            <li><a href="" >Blog</a></li>
            <li><a href="" >Sobre Mi</a></li>
            <li><a href="#contacto" >Contactame</a></li>
            <li><a href="" >GitHub</a></li>
        </ul>

    </nav>
</header>

    
<div id="footer" > © 2021 por Miguel Ivan Sanchez Sanchez. <b id="derecho">Todos los derechos reservados.</b>
    
</body>
```

[👆](#contenido)

---

## Sintaxis de una etiqueta

- Por lo general una etiqueta abre y otra cierra sin embargo hay algunas que no como la etiqueta br pero la sintaxis es similar en casi todas algunas requieren obligatoriamente un atributo

```html

<!-- Esta es la sintaxis de un comentario -->
<p>Esta es la sintaxis de la mayoria de etiquetas una abre
    y otra cierra </p>

<a href="#" target="_blank">enlace </a> 
<!--esta etiqueta requiere de forma obligatoria su atributo href-->

```

[👆](#contenido)

---

## Atributos Generales

- Son atributos que tienen todas las etiquetas html.

- Este enlace te muestra  [la lista completa](https://www.notion.so/Html-06932351bf8247c8a28920649322d4b5#18b236291fdc4bb484030001950c11b0)

- los mas usados **id, class, title, hidden, Style**

```html
<p id="paf" class="parf-ma fer" title="soy un parrafo" style="color:red;">
soy una etiqueta comun 
</p>

```

[👆](#contenido)

## Etiquetas mas Usadas

---

```html
<!--head-->
<!--etiquetas para adaptabilidad del sitio a otro navegaador y ajuste de resolucion y caracter-->
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!--head vincula elementos externos y titulo del sitio-->
<link rel="icon" href="img/feo.ico">
<link rel="stylesheet" href="style/styles.css">
<title>Miguel</title>
<!--body-->
<h1>Titulos hasta el h6<h1>
<div>Elemento en bloque comodin para estilos</div>
<p>parrafo o texto</p>
<input type="text" placeholder="Asunto" required>
<strong>Negrita representa importancia para el navegador    </strong>
<br><!--salto de linea-->
<style></style>
<script></script>
```

[👆](#contenido)

---

## Elementos externos

- Un documento html puede contener de todo solo se necesita documentarse y averiguar la implementacion. A continuacion algunos elementos.

### Imagenes

- src: direcion de la imagen si esta en nuestra ordenador o si esta en internet.

- width para el acho.

- alt en caso que la imagen no se pueda cargar o encotrar.

```html
 <img src="img/clik.jpg" width="500px" alt="F">
```

[👆](#contenido)

---

### Enlaces

- href : enlace de redireccionamiento
  
- target : donde mostrar el resultado del enlace

```html
  <a href="blog.html" target="_blank"> Blog</a>
```

[👆](#contenido)

---

### Listas

- ol: ordenadas 1,2,3,...
- ul : desordenadas . . .
- sea cual sea listas li para cada item

```html
<ol>
    <li>A</li>
    <li>B</li>
    <LI>C</LI>
</ol>

<ul>
    <li>javaScript</li>
    <li>React</li>
    <li>Angular</li>   
</ul>
```

[👆](#contenido)

---

## Multimedia

- Por el momento simple solo la direccion del archivo y controls

```html
<video src="mine.mp4"  controls ></video>
<!--Puede ser independiente en este caso de un archivo mp4 -->
<audio src="mine.mp4"  controls ></audio>
```

[👆](#contenido)

---

## Iframe

- una especie de web dentro la web xd

```html

<!--ESTA ETIQUETA LA GENERA GOOGLE MAP PARA INSERTARLA EN TU WEB-->
  <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d651.1633020410056!2d-77.04261658147952!3d-12.043162857500466!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8cd239a7ca3%3A0xe243b2147f189a1b!2sMetro%20Plaza%20Castilla!5e0!3m2!1ses-419!2spe!4v1614391118514!5m2!1ses-419!2spe" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

  <!--ESTA ETIQUETA LA GENERA YOUTUBE PARA INSERTARLA EN TU WEB-->
    <iframe width="560" height="315" src="https://www.youtube.com/embed/ZEyjjcuzkyw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 
 <!--ESTA ETIQUETA LA GENERA YO-->
<iframe src="https://carlosazaustre.es/blog" frameborder="0" width="450px" height="450px"></iframe>

```

[👆](#contenido)

---

## Formularios

- Envio de datos conceptos atributos orientados al back-end
- Compuesto de por las etiquetas **form y Imput**.

### Principales atributos

- action : define la accion que se realiza al momento de enviar los datos
- method : tiene get y post para el envio de informacion
- target : despues de enviar, donde se vizualiza la redireccion
- autocomplete : para que se pueda sugerir respuesta a los input

```html
<form method="GET" action="/HTML/example.html" target="_blank">
<!--etiquetas input/label-->
</form>
```

[👆](#contenido)

---

#### Modelo de form

```html
 <form method="GET" action="/HTML/example.html" id="form1" autocomplete="on">
        <fieldset>
            <legend>hola mundo</legend>
            <input type="text" name="usuario" id="usuario" placeholder="name" required><br>
            <br>
            <input type="text" name="lastname" id="lastname" required autocomplete="off" ><br>
            <br>
            <input type="email" name="email" id="email" required  ><br>
            <br>
            <input type="submit" name="" id="" value="subir">
        </fieldset>       
    </form>
```

[👆](#contenido)

---

### Input

- Existen diversos tipos de input

#### Atributos para input comunes

- **placeholder** : es un texto que ayuda a los input que piden una cadena de texto como un texto fantasma

- **required** : Hace obligatorio completar el input
- **name** : hace referencia al envio de datos por el metodo get en la url
- **autofocus** : redirecciona al input al cargar la pagina
- **type** : especifica el tipo de input
- **value** : valor inicial para el input

##### **Ejemp**

```html
<!--EL ORDEN NO IMPORTA CREO DX -->
<!-- Aca no utilzo el atributo value pq al tener el placeholder no se notaria xD-->
<input type="text" name="usuario" id="usuario" autofocus placeholder="name" required><br>

<input type="email" name="email" id="email" autofocus value="example@gmail.com" required><br>
```

[👆](#contenido)

---

#### Atributos para input poco comunes

- **redonly** : estable el input en solo lectura
- **disabled** : deshabilitado el input
- **maxlength** : maximo de caracteres
- **pattern** : especifica expresiones regulares, aunque por lo que veo ayuda a dar formato a las entradas  
- **form** : ayuda a vincular otro input si se encuentra fuera del form a traves del id del form al cual se le quiere vincular xDX
  
##### **Ejemplo**

```html
<form id="fom1">
     <fieldset>
            <legend>hola mundo</legend>
            <input type="text" name="usuario" id="usuario" placeholder="name" required><br>
            <br>
            <input type="text" name="lastname" id="lastname" required autocomplete="off" ><br>
            <br>
            <input type="email" name="email" id="email" required  ><br>
            <br>
            <input type="submit" name="" id="" value="subir">
        </fieldset>  

</form>


<!--visible y deshabilitado-->
<input type="text" name="usuario" id="usuario" value="Juanito" redonly disabled><br>
<!--maximo 8 caracteres-->
<input type="password" name="password" id="password"  maxlength="8" placeholder="********" required><br>

<!--asocio este input con el form de arriba por el id
pattern para dar formato al texto
by:w3school
-->
 <input type="tel" id="phone" name="phone" placeholder="123-435-678"
pattern="[0-9]{3}-[0-9]{3}-[0-9]{3}" required form="fomr1"><br>

```

[👆](#contenido)

---

#### Ejemplos de input poco vistos

```html
<!--select simple-->
<select name="paises" >
    <option value="mx">mk</option>
    <option value="pe">s</option>
    <option value="us">s</option>
    <option value="co">s</option>
</select>
<!--checkbox y radio-->
<input type="radio" name="gender" value="man">
<label for="man">man</label>
<input type="radio" name="gender" value="woman">
<label for="woman">woman</label>
<input type="checkbox">
<input type="week" alt="ftp" >
<!--envio-->
<input type="submit" value="Submit">
<!--rango del -10 al 50 avanza de 2 en 2 con valor inicial en 0-->
<input type="range" id="a" name="rango" value="0" min="-10" max="50" step="2">
<!--otra lista -->
<input list="browsers" required value="brave"name="browsers">
   <datalist id="browsers">
        <option value="Internet Explorer">
        <option value="Firefox">
        <option value="Chrome">
        <option value="Opera">
        <option value="Safari">
    </datalist>

```

[👆](#contenido)

---

## Paginas recomendadas

- etiquetas con ejemplos [htmlreference](https://htmlreference.io/)

## End

💜 **Hecho con amor**

[👆](#contenido)
