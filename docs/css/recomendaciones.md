---
id: recomendaciones
title: Recomendaciones
---


* Usar `margin-left` y `margin-rigth` con valor `auto` para centrar
  ```css
  .item { 
    margin-left: auto;
    margin-rigth: auto;
  }
  ```
Tratar de no comprometer el margin top y margin bottom
  ```css
  margin: 0 auto;
  ```

* En el caso de selectores agrupados, se recomienda separar en lineas diferentes. Ejm:
  ```css
  .title,
  .subtitle {
    color: green;
  }
  ```

* Usar `box-sizing` Para que se tome el valor asignado
  ```css
  * {
    box-sizing: border-box;
  }
  ```

* Utilizar el inspeccionar del navegador para hacer un seguimiento de estilos y no solo apoyarse de *Styles*, sino de *Computed*.

  ![ejemplo](../../static/img/css/imagen07.jpg 'ejemplo')

* Usar `inherit` para heredar propiedades de un elemento padre a un elemento hijo. Un ejemplo clásico de uso es en los enlaces ya que los navegadores le colocan asignan color azúl por default.
  ```html
  <p class="text">texto<a href="#">link</a></p>
  ```
  ```css
  .text { color: black; }
  .text a { color: inherit; }
  ```

## Malas prácticas

* Usar id como selectores, porque no se puede reutilizar
* Utilizar el `!important`, a menos que no te haya quedado de otra.
* Utilizar la especificidad, lo recomendable es usar clase o en todo caso usar máximo 02 niveles de especificidad. Aunque existen casos donde la especificidad aumenta, esto suele suceder al usar pseudo - clases como `:after`, `:before`, `:last-child`. Ejemplo de sass:

  ![ejemplo](../../static/img/css/imagen06.jpg 'ejemplo')

## Links de aportes

* **Calcular tamaño de pantalla según dispositivo** [http://viewportsizes.mattstow.com/mine/](http://viewportsizes.mattstow.com/mine/)
* **Obtener códigos de color Hex, RGB y HSL** [https://htmlcolorcodes.com/es/](https://htmlcolorcodes.com/es/)
* **Calculadora de especificidad**: [https://specificity.keegan.st/](https://specificity.keegan.st/)
* **Generar prefijos según navegadores** [https://autoprefixer.github.io/](https://autoprefixer.github.io/)
