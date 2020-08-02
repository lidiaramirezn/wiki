---
id: math
title: Math
---

Es un objecto que tiene propiedades y métodos para constantes y funciones. 

Me centraré en los métodos que más he usado

## Métodos

### Math.round()

Permite redondear según al número entero más cercano

```javascript
Math.round(10.42); // retorna 10
Math.round(10.5); // retorna 11
Math.round(10.78); // retorna 11
```

### Math.floor()
Permite redondear hacia abajo

```javascript
Math.floor(10.42); // retorna 10
Math.floor(10.5); // retorna 10
Math.floor(10.78); // retorna 10
```

### Math.ceil()

Permite redondear hacia arriba

```javascript
Math.ceil(10.42); // retorna 11
Math.ceil(10.5); // retorna 11
Math.ceil(10.78); // retorna 11
```

### Math.random()
Devuelve valor aleatorio entre 0 y 1,  Usualmene se multiplica otro valor. Ej: Si deseo obtener valores entre (0 y 20)

```javascript
Math.round(Math.random() * 20)
```