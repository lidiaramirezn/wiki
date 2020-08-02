---
id: selectores
title: Selectores
---

En esta sección colocaré ejemplos centrandome en los tipos de selectores que poco uso y que de vez en cuando olvido existen u olvido sintaxis.

## Selectores básicos

Existen diferentes tipos de selectores:

* Selectores de etiqueta
* Selectores de clases
* Selectores de ID
* Selector universal

Información: [https://www.eniun.com/selectores-css-tipos/](https://www.eniun.com/selectores-css-tipos/)

## Selectores  basados en relaciones (relationships)

### Selector hijo directo:
Se utiliza para seleccionar un elemento que es hijo directo de otro elemento y se indica mediante el "signo de mayor que" (>):

```css
.item > a {
  text-decoration: none;
}
```

### Selector hermano siguiente (Adyacente): 
Se emplea para seleccionar elementos que en el código HTML de la página se encuentran **justo a continuación** de otros elementos. Su sintaxis emplea el signo `+` para separar los dos elementos. .Ejm:

```css
.title1 + .subtitle {
  color: blue;
}

.title2 + .subtitle {
  color: red;
}
```

### Selector hermanos siguientes
El combinador `~` selecciona hermanos. Esto quiere decir que el segundo elemento sigue al primero (no necesariamente de forma inmediata)

[![ejemplo](../../static/img/css/imagen01.jpg 'ejemplo')](https://codepen.io/lidiaramirezn/pen/LYpggWL)

## Selector de atributos
Hace referecia a atributos de html. Estos selectores utilizan corchetes `[]`

[![ejemplo](../../static/img/css/imagen02.jpg 'ejemplo')](https://codepen.io/lidiaramirezn/pen/eYpPQNR)

### Selector de atributo comienza con 
Se representa `[attr^=value]`

[![ejemplo](../../static/img/css/imagen03.jpg 'ejemplo')](https://codepen.io/lidiaramirezn/pen/BaoGaWy)

### Selector de atributo termina con
Se representa `[attr$=value]`

[![ejemplo](../../static/img/css/imagen04.jpg 'ejemplo')](https://codepen.io/lidiaramirezn/pen/eYpQYMy)

### Selector de atributo que contiene
Representa elementos con un nombre de atributo cuyo valor contiene al menos una coincidencia de valor dentro de la cadena. Se representa `[attr*=value]`

[![ejemplo](../../static/img/css/imagen05.jpg 'ejemplo')](https://codepen.io/lidiaramirezn/pen/mdeQyoM)

Nota: Con este selector podemos evitar crear muchas clases. Ejemplo:
```html
<a class="button button-primary">Aceptar</a>
```