
En JavaScript, la forma de acceder al DOM es a través de un objeto llamado DOCUMENT, que representa el arbol DOM de la pagina o, mas concretamente, la pagina de la pestaña del navegador donde nos encontramos. En su interior pueden existir varios tipos de elementos, pero principalmente ELEMENT o NODE:

###### 1. ELEMENT no es mas que la representación genérica de una etiqueta: HTMLElement
###### 2. NODE es una más básica, la cual puede ser ELEMENT  o un nodo de texto.

Todos los **elementos HTML**, dependiendo del elemento que sean, tendrán un tipo de dato específico.
ejemplo:

#### HTMLDivElement : su etiqueta es: <div> </div> y  es una etiqueta divisora (en bloque).



#getElementById: Permite obtener un elemento del DOM por su atributo "id".


``` javascript
var elemento = document.getElementById("miElemento");

```

#getElementsByClassName: Obtiene una lista de elementos por su atributo "class".

```javascript
var elementos = document.getElementsByClassName("miClase");

```

#getElementsByTagName: Obtiene una lista de elementos por su etiqueta HTML.

```javascript
var elementos = document.getElementsByTagName("p");

```

#querySelector: Permite seleccionar un elemento utilizando selectores CSS.
``
```javascript
var elemento = document.querySelector("#miId");

```

#querySelectorAll: Selecciona múltiples elementos que coincidan con un selector CSS.
```javascript
var elementos = document.querySelectorAll(".miClase");

```

#createElement: Crea un nuevo elemento HTML.
```javascript
var nuevoElemento = document.createElement("div");

```

#appendChild: Agrega un elemento como hijo de otro elemento.

```javascript
var contenedor = document.getElementById("contenedor");
contenedor.appendChild(nuevoElemento);

```

removeChild: Elimina un elemento hijo de otro elemento.
```javascript
contenedor.removeChild(nuevoElemento);

```

#innerHTML: Permite acceder o modificar el contenido HTML de un elemento.
```javascript
elemento.innerHTML = "Nuevo contenido";

```

#innerText: Permite acceder o modificar el texto interno de un elemento.
```javascript
elemento.innerText = "Nuevo texto";

```

#setAttribute: Establece el valor de un atributo en un elemento.
```javascript
elemento.setAttribute("id", "nuevoId");

```

#classList: Permite agregar, quitar o verificar clases en un elemento.
```javascript
elemento.classList.add("nuevaClase");
elemento.classList.remove("viejaClase");
elemento.classList.contains("claseExistente");

```

#style: Modifica los estilos CSS de un elemento.
```javascript
elemento.style.color = "red";
elemento.style.backgroundColor = "blue";

```

#addEventListener: Permite agregar un evento a un elemento para responder a acciones del usuario.
```javascript
elemento.addEventListener("click", function() {
    // Código a ejecutar en respuesta al evento
});

```