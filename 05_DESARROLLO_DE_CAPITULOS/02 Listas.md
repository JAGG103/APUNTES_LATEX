# Listas

## ¿Cuales son las dos formas de listas que nos permite utilizar latex?

1. Listas númeradas

2. Listas no númeradas

_Es posible las anidaciones a las listas_

## ¿Qué comandos nos permite crear una lista númerada?

Creando un entorno

```latex
\begin{enumerate}
    \item text 1
    \item text 2
        % ...
\end{enumerate}
```

## ¿Qué comandos nos permite crear una lista no enumerada?

Creando un entorno

```latex
\begin{itemize}
    \item text 1
    \item text 2
        % ...
\end{itemize}
```

## ¿Como podemos utilizar simbolos en los items de una lista de forma personalizada?

Creando un entorno y en los comandos de item utilizar como opción el elemento que utilzaremos.

```latex
\begin{itemize}
    \item[a)] text 1
    \item[-] text 2
        % ...
\end{itemize}
```

_El incoveniente de esta forma es que tendremos que modificar todos las itemizaciones_

