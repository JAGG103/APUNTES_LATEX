# Bibliografia parte 2

## ¿Qué librerias deben de ser agregadas para poder hacer referencias a bibliografias?

1. csquotes : `\usepackage{csquotes}` Ajustar los procesos de latex del ingles al español

2. biblatex : `\usepackage{biblatex}` Gestion y creción de la bibliografia


## ¿Como se pueden colocar referencias a bibliografias en el documento?

1. En el __Preambulo__ debemos de utilizar el comando `\bibliography{}` para importar el archivo .bib que contiene las bibliografias. (Solo el nombre sin la extensión)

2. En el __Cuerpo__ del documento despues del ultimo capitulo debemos contruir la bibliografia con el comando `\printbibliography`

3. En el correspondiente parrafo de un capitulo donde queremos hacer una cita, utilizamos el comando `\cite{}` y como argumento el nombre nemonico de la referencia.


```latex
Durante las últimas tres décadas los modelos de comportamiento de peatones han captado un interés notable \cite{bib10, bib11, bib3, bib4}. Esto se debe en parte a que se han encontrado analogías no triviales entre el comportamiento de grupos de peatones con el comportamiento de gases y líquidos. También influye en este creciente interés el hecho de que actualmente existe una cantidad considerable de datos obtenidos mediante mediciones de flujo de peatones en video. Estos modelos peatonales pueden usarse como herramientas para el diseño y la planificación de las zonas peatonales, estaciones de metro o buses, grandes edificios, centros comerciales, etc\cite{bib8}.
```


## ¿Como podemos controlar el formato en que se hara la bibliografia?

Exiten dos forma de hacerlo desde el archivo main.tex donde importamos la libreria __biblatex__ agregando como opción: `\usepackage[  ]{biblatex}`

1. citestyle

2. style


Los posibles estilos:

- numeric
 
- alphabetic (respecto al autor: contracción del apellido y lugar de la bibliografia) 

- authoryear (ordenara por autor: nombre del autor y año)

`\usepackage[style=numeric]{biblatex}`

Podemos establecer Normas:

- apa

- mla (medical phsicological asociaton)

- ieee (institute of electrical and electronics engineer)

`\usepackage[style=apa]]{biblatex}`