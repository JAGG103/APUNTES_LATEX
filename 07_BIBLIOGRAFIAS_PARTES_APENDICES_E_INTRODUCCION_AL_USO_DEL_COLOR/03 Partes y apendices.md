# Partes y apéndices

Un trabajo de grado puede contener partes y las partes a su vez capitulos. Como tambien puede contener capitulos y que los capitulos contengan partes

En latex las partes son superiores a los capitulos


## ¿Cuál es el orden que por defecto tiene latex con la jerarquia de partes y capitulos?

Por defecto las partes contienen a los capitulos.

Podemos configurar latex para cambiar esta jerarquia a que los capitulos contengan partes.

_En la tesis podemos tener capitulos sin partes_


## ¿Como colocar partes en latex?

En el archivo .main utilizando el comando `part{}` y como argumento el nombre de la parte.

_Puede suceder que la parte se numere como romana, necesitamos arabigo, por lo tanto necesitamos colocar una nueva pagina y despues los comandos que configuran la numeración_

## En el escenario en el que necesitamos dos hojas en blanco consecutivas ¿Como se consigue?

Utilizando el comando `\newpage` dos veces, pero necesita haber un texto a la mitad, por lo tanto escribimos cualquier cosa y la pintamos de blanco.

```latex
% En el archivo .main
\usepackage[usenames]{color}

% ...

\newpage
\textcolor{white}{hola}
\newpage

```

## ¿Que libreria nos permite cambiar el color del texto?

color con la opción usenames.

`\usepackage[usenames]{color}` y con el comando `\textcolor{color}{text}`


## ¿Como podemos cambiar la jerarquia de partes y capitulos de latex?

En el __Preambulo__ colocamos los siguientes tres comandos

```latex
% ...

\makeatletter
\@addtoreset{chapter}{part}
\mateatother

% ...

```


De esta forma dentro de los capitulos podemos comenzar a crear partes utilizando el comando `\part{}`

_Si tratamos de colocar partes dentro de capitulos sin esta configuración errores podrian ser provocados en etapas posteriores_


<!-- Apendices -->


## ¿Qué es un apendice?

Es como un capitulo exteno que sirve de apoyo al trabajo.


## ¿Como podemos crear un apendice?

dentro del archivo .tex que corresponde al apendice debemos de colocar en la primera linea el comando `\appendix` y despues podemos agregar capitulos, partes, entre otros elementos de latex.

```latex
\appendix

\chapter{}

\section{}
```







