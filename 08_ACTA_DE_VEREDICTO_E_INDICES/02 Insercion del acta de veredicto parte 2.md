# Inserción del acta de veredicto parte 2

## ¿Como podemos colocar varias paginas de pdf en el documento?

1. Cargar la liberia: pdfpages 

2. En el correspondiente arhivo .tex colocamos el comando

```latex
\includepdf[pages=1]{Figuras/Acta.pdf}
```

Como argumento colocamos la ruta al documeto pdf, y como opción colocamos la pagina o el rango de paginas que deseamos cargar (pages=1)(pages=3-12)

_Esta forma no es la recomendable para colocar el acta de veredicto, ya que al colocar paginas de pdf de esta forma latex no las enumera, y debemos de hacer ciertos trucos colocados en el tutorial_