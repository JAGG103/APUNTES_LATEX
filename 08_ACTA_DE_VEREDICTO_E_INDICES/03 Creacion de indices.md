# Creación de índices

## ¿Qué comando nos permite crear el índice de forma automática?

`\tableofcontents`

_Índice generalmente va antes del capitulo 1_

## ¿Qué formato nos permite crear la lista de tablas y figuras?

```latex
\listoftables
\listoffigures
```

## ¿Qué comando nos permite configurar si se agregan las secciones, subsecciones o subsubsecciones al índice?

Utilizando el comando `\setcounter{tocdepth}{}`

```latex
\setcounter{secnumdepth}{3}
\setcounter{tocdepth}{3}
```

1. Argumento determina que elemento estamos configurando

2. Argumento es un numero entero del 0-3 

Estos dos comandos son complementarios, el primero permite definir la enumeración de los elementos mediante su jerarquia, el segundo nos permite configurar la visualización de estos elementos en la tabla de contenidos tambien dependiendo de sus jerarquia.


## ¿Qué comandos nos permiten hacer que las partes del preambulo se muestren el la TOC? (Table Of Content)

Dentro del archivo .tex

```latex
\chapter*{}
\addcountentsline{toc}{chapter}{nombre}
```

Los argumentos:

1. toc hace referencia a la tabla de contenidos

2. Aparecera en formato de capitulo

3. Nombre de la parte como aparecera en el índice

_Repetiremos esto para cada elemento que deseamos aparezcan el la toc_


## ¿Como podemos colocar un cierto tamaño y fuente al índice?

Cargarmos la libreria: fountenc

`\usepackage[T1]{fountenc}`

_T1 hace referencia a un formato para el índice_

