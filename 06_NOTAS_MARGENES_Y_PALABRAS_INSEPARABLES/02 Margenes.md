# Margenes

## ¿Que librerias son utiles para modificar los margenes de la pagina?

1. vmargin : `\usepackage{vmargin}`

2. geometry: `\usepackage[  ]{geometry}`

## ¿Como podemos modificar los margenes utilzando la libreria vmargin?

 vmargin : permite utilizar el comando `\setlenght{}{}` para

```latex
\usepackage{vmargin}

% dentro del preambulo
\setlenght{\textwidth}{150mm} % modificar el ancho del texto
\setlenght{\textheight}{215mm} % modificar la altura del texto
\setlenght{\oddsidemargin}{40mm} % el margen de la izquierda de las paginas impares
\setlenght{\evensidemargin}{40mm} % el margen de la izquierda de las pagina pares
\setlenght{\topmargin}{30mm} % el margen superior
```

## ¿Como podemos modificar los margenes utilizando la libreria geometry?

```latex
\usepackage[papersize={216mm, 330mm}, tmargin=15mm, bmargin=15mm, lmargin=15mm, rmargin=15mm]{geometry}
```

ó

```latex
\usepackage[a4paper]{geometry}
\geometry{top=2cm, bottom=2cm, left=4cm, right=2cm}
```