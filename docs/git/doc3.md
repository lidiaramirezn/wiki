---
id: doc3
title: Comandos relevantes de git
sidebar_label: Comandos git
---

**Versión de Git**
~~~
git version ó git --version
~~~

**Configuración global**
~~~
git config --global user.email correo@mail.com
git config --global user.name "nombre usuario"
~~~

**Mostrar información de configuración**
~~~
git config --list
~~~

**Crear repositorio Git** *(Paso 1)*
~~~
git init
~~~

**Estado del repositorio**
~~~
git status
~~~

**Agregar archivos al directorio local** *(Paso 2)*

~~~
git add nombre-archivo.extension // Agregar un archivo específico
git add . ó git add --all        // Agregar todos los archivos
~~~

**Eliminar del directorio local**
~~~
git rm --cached nombre-archivo.extension
git rm -f archivo.extension // Forzar un remove definitivamente
~~~

**Confirmar cambios** *(Paso 3)*
~~~
git commit -m "mensaje descriptivo"
~~~

**Agregar un archivo al último commit**
~~~
git add archivo-olvidado.extension
git commit --amend
~~~

**Agregar un archivo y reemplazar último commit**
~~~
git add archivo-olvidado.extension
git commit --amend 'Nuevo mensaje'
~~~

Si aparece el editor, solo colocar `:q!` para salir

**Conectar con repositorio remoto**
~~~
git remote add origin url-repositorio
~~~

**Visualizar la URL asociada a repositorio remoto**
~~~
git remote -v
~~~

**Subir cambios a un repositorio remoto** *(Paso 4)*
~~~
git push origin nombre-rama
~~~

**Actualizar las referencias remotas**
~~~
git pull origin nombre-rama
~~~

**Crear una rama**
~~~
git checkout -b nombre-rama
~~~

**Cambiar de una rama a otra**
~~~
git checkout nombre-rama
~~~

**Deshacer cambios, antes de hacer commit**
~~~
git checkout nombre-archivo.extension // de un archivo
git checkout -f  // varios archivos
~~~

**Borrar una rama**
~~~
git branch -D nombre-rama
~~~

**Cambiar de rama sin confirmar cambios**
~~~
git stash
~~~

**Regresar cambios**
~~~
git stash pop
~~~

**Obtener todas las ramas remotas a local**
~~~
git fetch origin
~~~

**Visualizar todas las ramas**
~~~
git branch
git branch -a
~~~

**Fusionar ramas**

Para ello hay que ubicarse en la rama que queremos dar merge para traer cambios (si hubieran) de otra rama
~~~
git merge otra-rama
~~~