# Tablas parte 1

## ¿Que comandos nos permiten crear una tabla en latex?

```latex

\begin{table}[]
    \centering
    \begin{tabular}{c|c}
         &  \\
         & 
    \end{tabular}
    \caption{Caption}
    \label{tab:my_label}
\end{table}

```

donde:

En las Opciones del inicio del entorno `\begin{table}[]` podemos colocar la posicion de la tabla en el documento (se puede usar el paquete "float")

En segundo lugar de los argumetos del comando `\begin{tabular}{}` podemos colocar la alineación del contenido y si queremos lineas verticales.

Los `&` separan las columnas y los `\\` separan las filas

Podemos colcoar el comando `\hline` para agregar lineas horizontales.

El comando `\caption{}` nos permite colocar una descripción de la tabla 

El comando `\label{}` agrega una etiqueta para referenciarla en el documento

## ¿Como podemos hacer que latex coloque tablas en lugar de cuadro al nombrar la table?

Agregando una segunda opción al cargar el paquete `\usepackage[spanish, es-tabla]{babel}`




