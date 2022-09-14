# Lab: Vinculando un archivos JavaScript externos

## Objetivos
- Vincular un archivo HTML (`index.html`) con un archivo JavaScript (`script.js`) utilizando el atributo `src` y la etiqueta `<script>`

## Introducción 
Los desarrolladore evitan mezclar código escrito en distintos lenguajes de programación. Por esta razón normalmente se guarda el código HTML, CSS, y JavaScript en archivos separados (los archivos HTML contienen solo código HTML,  los archivos CSS contienen solo código CSS, y los archivos JavaScript contienen solo código JavaScript).


## Funcionalidad del Código
En este lab crearas un documento javascript con la extensión `.js`

## Instrucciones 
Bifurca (fork) y clona (clone) este lab en tu entorno local. Navega a su directorio en la terminal, luego ejecuta el comando `code .` para abrir sus archivos en Visual Studio Code. 

1. Borra el código que creaste en la última lección (se encuentra al final del documento HTML). Básicamente el siguiente:

```
<script> 
   const flappyBird = document.querySelector("#flappy-bird")

   flappyBird.addEventListener("click", function() {
       alert("Hola desde el elemento <script>!")
   })
</script>
```

2. Crea un archivo `script.js` que se encuentre en la misma carpeta/directorio que tu archivo `index.html`

3. Agrega el siguiente código dentro de `script.js`

```
const flappyBird = document.querySelector("#flappy-bird")

   flappyBird.addEventListener("click", function() {
       alert("Hola desde script.js!")
   })
```

4. En tu archivo HTML dentro de `<head>` agrega un elemento `<script>` con el atributo src apuntando a `script.js`. Incluye el atributo `defer`.

```
<head>
   <title>Los lenguajes del navegador</title>
   <link rel="stylesheet" type="text/css" href="style.css">
   <script src="script.js" defer></script>
</head>
```

5. Guarda tus cambios (Archivo > Guardar)

6. Abre tu archivo html en el navegador. Da click sobre la imagen de flappy bird (en la parte inferior izquierda de la pagina web). Al dar click sobre ésta imagen te debe de aparecer una ventana con el mensaje `"Hola desde script.js!"`

7. Sube tus cambios a Github y envía por Canvas el enlace a tu repositorio.