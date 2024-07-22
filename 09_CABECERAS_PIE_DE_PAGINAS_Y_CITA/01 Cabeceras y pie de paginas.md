# Cabeceras y pie de páginas

## ¿Qué comando nos permite modificar el ancho de la cabecera de forma general?

En el preámbulo del documento colocar:

`\setlength{\headheight}{24pt}` antes de cualquier importación de librerias que trabajen con las cabeceras

## ¿Como podemos configurar cabeceras y pie de paginas en todas las hojas? 

1. Creamos un archivo .tex el cúal contendra estas configuraciones, debe contener los siguientes comandos:

```latex
% Configuración del ancho de la cabecera (Si no se configura puede dar problemas con la libreria fancyhdr)
\setlength{\headheight}{24pt}

% Importación de la libreria fancyhdr
\usepackage{fancyhdr}

% ----------------------------- [CONFIGURACIÓN PARA PAGINAS QUE NO SON INICIOS DE CAPITULOS ] -----------------------------------------
% Corchetes afecta paginas pares, llaves paginas impares, los capitulos siempre son paginas impares
\lhead[]{} 
\chead[]{}
\rhead[]{}
% Comando para modificar el grueso de la linea de la cabecera
\renewcommand{\headrulewidth}{1pt}

% Configuraciones para pie de paginas
\lfoot[\thepage]{Jhonatan Gomez}
\cfoot[]{}
\rfoot[Jhonatan Gomez]{\thepage}
% Configraciones para grueso de la linea en el pie de página
\renewcommand{\footrulewidth}{1pt}

% Afectamos las páginas con los cambios realizados
\pagestyle{fancy}

% ----------------------------- [CONFIGURACIÓN PARA LAS PAGINAS DE INICIO DE CAPITULOS ] ---------------------------------------------


\fancypagestyle{plain}{
    \fancyhead[L]{}
    \fancyhead[C]{}
    \fancyhead[R]{}
    \fancyfoot[L]{Jhonatan Gomez}
    \fancyfoot[C]{}
    \fancyfoot[R]{\thepage}
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{1pt}
}
```

2. Agregamos ese archivo .tex en el __Preambulo__ del documento justo antes del cuerpo del mismo.

```latex
% ...
\input{path/cpp.tex}

\begin{document}
% ...
\end{document}
```


## ¿Como podemos configurar cabeceras y pie de páginas en capitulos especificos?

1. Debemos contar con los siguientes comandos:

```latex
\lhead[]{}
\chead[]{}
\rhead[]{}
```

Se espera poder colocar el nombre del capitulo acompañado o utilizando los siguientes comanodos:

- `\thechapter` nos regresa el número del capítulo
- `\leftmark` nos regresa el nómbre del capítulo así como su número
- `\rightmark` nos regresa el nombre de la primera sección asi como su número

2. Colocar los comandos despues de la aparición de la parte o elemento

```latex
\listoftables
\lhead[Lista de Tablas]{}
\chead[]{}
\rhead[]{Lista de Tablas}
```

_Esto puede ir en el cuerpo del documento_

_Si existe algun error, podemos intentar colocar esos comandos despues de aquellos que configuran su aparición en el indice o numeración_


