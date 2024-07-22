# Subfiguras

En ocasiones necesitamos que una figura albergue mas dos figuras

## ¿Que paquete es necesario cargar para tener subfiguras?

El paquete: subfig utilizando `\usepackage{subfig}`

## ¿Como podemos cargar subfiguras?

Similar a como incluimos imagenes, pero incluytendo los comandos `\subfloat[]{}`

```latex

\begin{figure}
    \centering
    \subfloat[Descripción de subfig 1]{ \includegraphics[width=]{path/name} }
    \subfloat[Descripción de subfig 2]{ \includegraphics[width=]{path/name} }
    % ....
    \subfloat[Descripción de subfig 3]{ \includegraphics[width=]{path/name} }
    \caption{Descripcion del conjunto de figuras}
    \label{fig:enter-label}
\end{figure}

```

De esta forma agregamos imagenes de forma horizontal y seguidas, para colocarlas de forma vertical basta con separar con un salto de linea cada comando `\subfloat[]{}`

```latex

\begin{figure}
    \centering
    \subfloat[Descripción de subfig 1a]{ \includegraphics[width=]{path/name} }
    \subfloat[Descripción de subfig 1b]{ \includegraphics[width=]{path/name} }

    \subfloat[Descripción de subfig 2a]{ \includegraphics[width=]{path/name} }
    \subfloat[Descripción de subfig 2b]{ \includegraphics[width=]{path/name} }
    \caption{Descripcion del conjunto de figuras}
    \label{fig:enter-label}
\end{figure}

```