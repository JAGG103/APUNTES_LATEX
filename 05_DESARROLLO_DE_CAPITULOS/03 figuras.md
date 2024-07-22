# Figuras

## ¿Que comandos nos permite colocar figuras en latex?

Utiliando un entorno con el parametro figure.

```latex

\begin{figure}
    \centering
    \includegraphics[]{}
    \caption{Caption}
    \label{fig:enter-label}
\end{figure}

```

donde:

El primero comando `\centering` dentro del entorno hace referencia a la posición de la imagen en la linea
El segundo `\includegrafics[]{}` es para colocar el tamaño (width=0.3\textwidth) el path de la figura y su nombre
El tercero `\caption{} `es para agregar la descripción de la imagen
El cuarto `\label{label}` es para colocar una etique a la imagen para futuras referencias en el texto `\ref{label}`

## ¿Como podemos sugerir a latex una posición en la pagina para colocar la figura?

En el primer comando que crea el ambiente, al final colocamos un campo para opciones [ ]

`\begin{figure}[]`

dentro podemos escribir:

- t : Parte superior
 
-  b : Parte inferior

- h : En la posición actual

_Si latex considera que se esta desperdiciando recursos importantes para la claridad y formato profesional entonces podra decidir si hacer caso omiso a nuestra sugerencia_

## ¿Como podemos agregar mayor peso a nuestra sugerencia de la posición de una figura?

Agregando un signo de exclamación `!` despues de la letra de la posición.

`\begin{figure}[h!]`

_Pero aun utilizando esta opción latex puede hacer caso omiso a la orden_

## ¿Que paquete nos permite forzar a latex a colocar la imagen en la posición solicitada?

1. Cargando el paquete: float `\usepackage{float}`

2. y utilizando las letras: H,T ó U para colocarlas en la posición donde aparece, superior o inferior.

