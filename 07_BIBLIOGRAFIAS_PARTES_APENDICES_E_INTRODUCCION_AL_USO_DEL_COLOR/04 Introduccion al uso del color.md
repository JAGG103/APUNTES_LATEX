# Introducción al uso del color

## ¿Cuales son los colores basicos de latex para cambiar de color a un texto?

```latex
\textcolor{white}{Text}
\textcolor{black}{Text}
\textcolor{yellow}{Text}
\textcolor{green}{Text}
\textcolor{blue}{Text}
\textcolor{red}{Text}
\textcolor{cyan}{Text}
```

## ¿Como podemos pintar parrafos completos?

Utilizando Bloque + Orden

```latex
{
    \color{  }
}
```

Podemos utilizar tanto los colores basicos de latex, como aquellos de un modelo, o creados y definidos por el usuario

## ¿Como podemos utilizar los colores de un modelo?

Los 3 módelos disponibles son: 

- rgb (red, green, blue)
- cmyk (cyan, magen, yellow, black)
- grey 

utilizando `\textcolor[]{}{}`

Donde cada modelo tendra sus tuplas cada canal entre 0 y 1 para determinar proporcion del color:

```latex
\textcolor[rgb]{0.5,0.5,0.9}{Text}


\textcolor[cmyk]{0.6,0.7,0.9}{Text}


\textcolor[grey]{0.9}{Text}
```


## ¿Como podemos definir un color nuevo?

Utilizando el comando `\definecolor{}{}{}`

1. Atributo el nombre del color (label)

2. El nombre del modelo

3. La escala de los canales

_podemos utilizadnos tanto en el comando textcolor, color llamando a definecolor y su label_

## ¿Que comando nos permite cambiar el color de una pagina?

`\pagecolor{}`

Podemos utilizar tanto los colores basicos de latex, como aquellos de un modelo, o creados y definidos por el usuario

_Esto pintara todas las paginas siguientes, pero podemos limitarlo a unas cuantas definiendo el limite superior como blancas de nuevo_


## ¿Como podemos crear cajas de color?

Utilizando el comanod `\colorbox{}{}`

Donde los atributos:

1. El nombre del color

2. El Texto dentro de la caja

Podemos utilizar colores basicos, colores de modelos o colores nuevos ya definidos.

Tambien podremos colocar un contorno a la caja colocando los siguienes comandos antes del comando nuevo `\fcolorbox{}{}`

```latex
\setlenght{\fboxrule}{3pt}
\fcolor{red}{yellow}{Caja de fondo amarillo y contorno rojo}
```



