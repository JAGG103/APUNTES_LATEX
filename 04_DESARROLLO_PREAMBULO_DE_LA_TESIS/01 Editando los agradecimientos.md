# Editando los agradecimientos

## ¿Que comando nos permite agregar un espacio vertical determinado?

Espacios verticales : `\vspace{}` Comando + Argumento

_Se pueden colocar cualquier cantidad de espacio en cualquiera de las unidades estudiadas en este capítulo_

## ¿Que comando nos permite mover un parrafo a la derecha, izquierda o centro?

Entorno

- Izquierda 

```latex
\begin{flushleft}
Text
\end{flushleft}
```

- Derecha 

```latex
\begin{flushright}
Text
\end{flushright}
```

- Centro

```latex
\begin{center}
Text
\end{center}
```

_Podemos anidar otros comandos dentro del entorno creado, por ejemplo si queremos agregar un perfil_

```latex
% Ejemplo
\begin{flushright}
\textit{\large A usted que me lee y escucha\\ con la convicción de aprender \ldots}      
\end{flushright}

```


## ¿Que comando nos permite agregar tres puntos suspensivos en latex?

`\ldots`

