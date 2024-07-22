# Etiquetas y referencias

Repasar el comando `\label{}` y el comando `\ref{}`


## ¿Que comando nos permite crear un label a un capitulo, seccion, subsección o entorno?

Despues de su comando de apertura escribir el comando `\label{}`

## ¿Para que sirven los labels y las referencias?

Para hacer una conexión de forma automatica de la enumeración de una figura, tabla, capitulo, seccion, subsección entorno con una referencia.

Dicha referencia debe de ser unica e irrepetible.

_Se puede crear un label a un capitulo para poder referenciarlo en otra parte_

```latex
\chapter{capitulo 1}\label{cap1}
```