# Insección del acta de veredicto parte 1

## ¿Como podemos cargar una imagen de fondo en todo el documento?

1. Cargar el paquete: background usando el comando `\usepackage[pages=All]{background}`

donde se le coloca como valor a la opción pages: All

2. Configuraremos el formato con los comandos siguientes despues de la importación de la libreria en el preambulo:

```latex
\backgroundsetup{
    scale=1, % Porcentaje de 0 a 1
    color=black, % Color para opacidad
    opacity=0.4,  % Porcentaje de opacidad
    angle=0, % Rotación
    contents={\includegraphics[width=\paperwidth, height=\paperheight]{Figures/Acta.pdf}} % Podemos hacerlo con formatos jpeg, png
}
```
_Se cargara en todas las imagenes del documento_

## ¿Como podemos cargar una imagen como fondo en solo una o algunas paginas del documento?

1. Cargar el paquete: background usando el comando `\usepackage[pages=some]{background}`

2. Configuraremos el formato con los comandos siguientes despues de la importación de la libreria en el preambulo:

```latex
\backgroundsetup{
    scale=1, % Porcentaje de 0 a 1
    color=black, % Color para opacidad
    opacity=0.4,  % Porcentaje de opacidad
    angle=0, % Rotación
    contents={\includegraphics[width=\paperwidth, height=\paperheight]{Figures/Acta.pdf}} % Podemos hacerlo con formatos jpeg, png
}
```

3. La pagina donde queremos se coloque el fondo vamos al poner el comando `\BgThispage` despues del comando del capitulo.

_El acta de veredicto normalmente se encuentra despues de la portada_

## ¿Como podemos agregar el acta de Veredicto despues de la portada?

(A) Colocandola como fondo de la pagina

1. Cargar el paquete: background usando el comando `\usepackage[pages=some]{background}`

2. Configuraremos el formato con los comandos siguientes despues de la importación de la libreria en el preambulo:

```latex
\backgroundsetup{
    scale=1, % Porcentaje de 0 a 1
    color=black, % Color para opacidad
    opacity=0.4,  % Porcentaje de opacidad
    angle=0, % Rotación
    contents={\includegraphics[width=\paperwidth, height=\paperheight]{Figures/Acta.pdf}} % Podemos hacerlo con formatos jpeg, png
}
```

3. Creamos una especie de capitulo que contendra el acta, y lo cargamos en el lugar que le corresponde

```latex
% Acta.tex
\chapter*{}

\BgThispage
```

4. Corregimos la numeración la cual al tratarse de parte del preambulo del documento, debe de estar en numeros romanos

```latex
% Acta.tex
\chapter*{}
\pagenumbering{Roman}
\setcounter{page}{1}
\BgThispage
```

_Podemos controlar el formato del fondo modificandolo en el preambulo_

(B) Cargandola como una imagen utilizando los entornos para figure

```latex
\begin{figure}[h!]
    \centering
    \includegraphics[with=\textwidth]{Figuras/Acta.pdf}
\end{figure}
```

_Podemos colocar un libro en pdf, tomara y mostrara la primera pagina_

_El problema de utilizar esta forma es que va a respetar los margenes, y los espacios que el pdf ya contenga_

