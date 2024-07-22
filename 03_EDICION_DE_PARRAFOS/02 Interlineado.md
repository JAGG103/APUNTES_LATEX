# Interlineado

## ¿Cuáles son las dos formas de moficar el interlineado?

1. Utilizando el comando `\renewcommand{\baselinestretch}{2}` (Segundo atributo es el numero de espacio de interlineado)

2. Utilizando e Importando la libreria `setspace` (Nos proporciona 4 nuevos comandos) 

```latex
\documentclass{book}

% ------------------ Paquetes
\usepackage{setspace}

% ------------------ Preambulo

\doblespacing % Interlineado doble
\onehalfspacing % Interlineado 1 y medio
\singlespacing % Interlineado simple
\spacing{1.5} % Interliineado variable

% ----------------- Cuerpo del documento
\begin{document}

\end{document}
```