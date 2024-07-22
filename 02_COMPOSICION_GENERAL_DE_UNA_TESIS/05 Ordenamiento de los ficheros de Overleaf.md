# Ordenamiento de los ficheros de Overleaf

## ¿Para que se recomienda hacer esto?

Conforme el documento crezca tambien lo hara el número de lineas, por lo cual es recomendable tener las secciones separadas en diferentes archivos .tex para cada parte.

```latex
%--------------- CLASE DE DOCUMENTO
\documentclass[a4paper, 12pt, oneside, openright]{book}

%--------------- LIBRERIAS
\usepackage[utf8]{inputenc}
\usepackage[spanish]{babel}

%--------------- PREAMBULO
\title{Thesis}
\author{Jhonatan}
\date{\today}

%--------------- CUERPO
\begin{document}

\end{document}
```

## ¿Qué comando nos permite cargar archivos.tex al archivo main de latex?

`input{name.text}`

Este comando nos permite colocar de forma secuencias el contenido del archivo.tex en el archivo main

