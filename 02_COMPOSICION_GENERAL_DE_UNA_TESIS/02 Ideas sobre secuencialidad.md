# Ideas sobre secuecialidad

## El compilador de latex ¿Como análiza los comandos?

De forma secuencial de arriba a abajo.

Se ejecutan las acciones o se crean los elementos en ese orden.

## ¿Qué comando nos permite crear una nueva pagina en latex? Vacia y sin Enumeración

```latex
\newpage % COMANDO : crea una nueva pagina
\thispagestyle{empty} % COMANDO : permite colocar ese estilo a la pagina creada
```

_Esto es util para la pagina despues de la portada, la cual debe estar vacia y sin enumeración_

![](figures\newpage.png)
