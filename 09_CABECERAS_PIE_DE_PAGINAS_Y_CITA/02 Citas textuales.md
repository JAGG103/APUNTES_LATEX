# Citas textuales

## ¿Cúales son los dos tipos de citas textuales que podemos utilizar en latex?

1. Citas textuales cortas (Se colocan dentro de los parrafos)

2. Citas textuales largas (Se colocan en un nuevo parrafo, centradas y con formato especifico)

## ¿Cómo colocar citas textuales cortas?

1. Nos posicionamos en el texto de interes

2. Utilizamos la forma: 

```latex

``Texto al que se quiere referenciar'' (\citeauthor{label}, \citeyear{label}:n_pagina)

```

## ¿Como conseguimo que una cita no sea cortada/separada por latex?

Utilizando el comando `~\mbox{}`

```latex
~\mbox{``Texto al que se quiere referenciar'' (\citeauthor{label}, \citeyear{label})}
```

## ¿Como podemos crear citas textuales largas?

```latex
\begin{center}
    \begin{minipage}{0.9\linewith} % Margenes laterales de la cita textual
        \vspace{5pt}
        {
            \small
            Texto que tendra la cita textual larga
        }
        \begin{flushright}
        (\citeauthor{label}, \citeyear{label}:n_page)
        \end{flushright}
        \vspace{5pt}
    \end{minipage}
\end{center}
```