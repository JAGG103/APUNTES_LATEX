# Comandos de estilo de pagina y clase documento

## ¿Cuáles son los atributos posibles para el comando \thispagestyle ?

- `empty` (Estilo donde las paginas no contiene encabezados, pie de paginas y numeración)

- `plain` (Solo escribe enumeración de cada pagina)

- `heading` (Montar en las cabezeras la sección y el numero de paginas)

- `myheading` (Determinar lo que queremos que se muestre en la cabezera)

## ¿Como puedo modificar el estilo de todas las hojas de mi documento?

Utilizando el formato `\pagestyle{}` antes de la apertura del cuerpo del documento

```latex
\pagestyle{}
\begin{document}

\end{document}
```

utilizando alguno de los atributos estudiados.

_Al utilizarlo empty en todo el documento, los que contienen inicios de capitulos si las enumera_


## ¿Cuáles son los atributos posibles para el comando \documentclass ?

- `article` (Articulos cientificos)

- `book` (Tesis)

- `report` (Reportes tecnicos)

- `memoir` (Memorias)

- `beamer` (Diapositivas)

## ¿Cúales son las opciones del comando \documentclass ?

Podemos utilizar multiples opciones separandolas por coma `,`. Se utilizan para determinar el tamaño de las paginas, fuente, impresión a una o doble cara y donde deben de empezar los capitulos (impar).

### Determinar los tamaños de las paginas

- a4paper

- a5paper

- b5paper

- legalpaper

- executivepaper

- letterpaper (predeterminado)

```latex
\documentclass[letterpaper]{book}
```

### Determinar el tamaño de la fuente

- 12pt 

```latex
\documentclass[letterpaper, 12pt]{book}
```

### Determinar la impresión a una o doble cara

- oneside

- twoside

```latex
\documentclass[letterpaper, 12pt, twoside]{book}
```

### Determinar en que pagina deberan de iniciar los capitulos

- openright

- openany

```latex
\documentclass[letterpaper, 12pt, twoside, openright]{book}
```

