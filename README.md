# Fundamentos de JavaScript
- [Fundamentos de JavaScript](#fundamentos-de-javascript)
  - [Introducción](#introducción)
    - [Empezamos con JavaScript](#empezamos-con-javascript)
  - [Variables](#variables)
  - [Metodos de visualizacion de informacion](#metodos-de-visualizacion-de-informacion)
    - [Funcion `alert()`](#funcion-alert)
    - [Funcion `console.log()`](#funcion-consolelog)
    - [Funcion `document.write()`](#funcion-documentwrite)
  - [Tipos de datos](#tipos-de-datos)
  - [Operadores](#operadores)
## Introducción
Teniendo en cuenta que `HTML` es un lenguaje de enmarcado que nos va a servir para dar estructura a la informacion que queremos presentar mediante una pagina web y que `CSS` nos ayuda a dar estilos a esa informacion de tal forma que podamos mostrar de una forma estetica y maquetar nuestra web, `JavaScript` es un lenguaje de programación que se puede usar para volver interactiva nuestra web, con `JavaScript` podemos agruegar logica y dinamismo a nuestro contenido del lado del cliente, agregar botones, validar formularios, cambiar el color de texto, el color de fondo, y muchas cosas mas, basicamente sin `JavaScript` nuestra web seria estatica y no podriamos cambiar el contenido.

### Empezamos con JavaScript
Lo primero que debemos hacer es crear un archivo `HTML` con la estructura basica para hacer el llamado de javscript, para lo cual tendremos 2 formas de trabajar:

* Mediante el uso de la etiqueta `<script>`:
    
```html 
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    <!-- Aqui va nuestro codigo html --> 

<script>
    // Aqui va el codigo de JavaScript
    alert("Hola mundo");
</script>
</body>
</html>
```
* Mediante el uso de la etiqueta `<script>` pero utilizando el atributo `src`:  
    Ejemplo: `<script src="js/script.js"></script>`
```html 
<!DOCTYPE html>
<html lang="en">
<head>
    <script src="js/script.js"></script>
    <title>Document</title>
</head>
<body>
<!-- Aqui va nuestro codigo html --> 
</body>
</html>
```
## Variables
Las variables son contenedores en donde guardamos informacion que podemos utilizar en nuestro codigo de JavaScript. 

Para crear una variable debemos utilizar la palabra reservada `var` (existen otro tipo de variables en las cuales utilizaremos `let` o `const`) y luego el nombre de la variable, para asignarle un valor a la variable debemos utilizar la palabra reservada `=` y luego el valor que queremos asignarle a la variable.  
Ej.:
```javascript
// Creacion y asignacion de una variable
var nombre = "Juan";
```
Ademas podemos hacerlo en 2 fases, la primera es crear la variable y la segunda es asignarle un valor a la variable.

```javascript
// creacion de la variable
var nombre;
// asignacion de la variable
nombre = "Juan";
```

Tambien podemos crear varias variables en una sola linea, para lo cual utilizaremos la palabra reservada `var` y luego el nombre de la variable y luego una coma y luego el nombre de otras variables y asignar su valor posteriormente.

```javascript
// creacion de variables
var nombre, apellido;
// asignacion de valores a las variables
nombre = "Juan";
apellido = "Perez";
```

## Metodos de visualizacion de informacion
A continuacion veremos los metodos de visualizacion de informacion de las variables que podemos utilizar para mostrar informacion en nuestra pagina web, o `consola` del `JavaScript`.

### Funcion `alert()`
La funcion `alert()` nos permite mostrar un mensaje en una ventana emergente.

```javascript
var variable = "Hola mundo soy un alert";
alert(variable);
```
Esto se ve asi:
![Funcion alert](./9_javaScript/img/funcionAlert.png)

### Funcion `console.log()`
La funcion `console.log()` nos permite mostrar un mensaje en la consola del navegador.

```javascript
var variable = "Hola mundo soy un console.log";
console.log(variable);
```
Esto se ve asi:
![Funcion console.log](./9_javaScript/img/funcionConsoleLog.png)

### Funcion `document.write()`
La funcion `document.write()` nos permite mostrar un mensaje en la pagina web escribiendo directamente en el `HTML`.

```javascript
var variable = "Hola mundo soy un document.write";
document.write(variable);
```
Esto se ve asi:
![Funcion document.write](./9_javaScript/img/funcionDocumentWrite.png)

## Tipos de datos
Los tipos de datos que podemos utilizar en JavaScript son:
  - Numericos
  - Cadenas de texto
  - Arreglos
  - Funciones
  - Booleanos
  - Objetos

```html 
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
<!-- Aqui va nuestro codigo html -->
<script>
    var numero = 7; // variable numerica
    var decimal = 7.5; // variable numerica decimal

    var cadena = "Hola"; // variable cadena de texto
    var cadena2 = '5'; // variable cadena de texto conteniendo un numero

    var arreglo = [1,2,3,4,5]; // variable arreglo

    var saludo = function(){ 
            console.log("Hola");
    } // variable funcion

    booleano = true; // variable booleana

    objeto = {
        nombre: "Juan",
        apellido: "Perez",
        edad: 25
    }; // variable objeto
</script>   
</body>
</html>
```

## Operadores