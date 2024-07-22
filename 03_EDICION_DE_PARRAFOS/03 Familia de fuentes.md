# Familia de fuentes

## ¿Cuáles son las 3 familias que latex permite utilizar?

1. Familia $\rm{roman}$

2. Familia $\sf{sanserif}$

3. familia $\tt{typewriter}$


## ¿Cuáles son las 3 formas editar las familias de fuentes?

1. Comando + Argumento : `\textrm{Text}`, `\textsf{Text}`, `\texttt{Text}`

2. Bloque + Orden : Utilizando bloques { } y el comando con la familia

```latex
\rmfamily
{
Este es un parrafo.
}
```

3. Entorno

```latex
\begin{rmfamily}
Este es un parrafo.
\end{rmfamily}
```

_Si utilizamos la forma entorno, si tenemos configurado un tipo de fuente para todo el documento, este bloque podra tener una fuente distinta que solo tendra efecto en este bloque_


## ¿Como podemos configurar una sola fuente para todo el documento?

Colocando el comando `\rmfamily`, `\sffamily` o `\ttfamily` en la primera linea despues del comando `\begin{document}`

