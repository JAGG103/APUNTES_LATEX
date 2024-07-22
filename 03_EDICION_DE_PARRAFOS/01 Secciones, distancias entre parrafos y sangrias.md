# Secciones, distancias entre parrfos y sangrias

## ¿Como podemos modificar el espacio entre parrafos y la sangria de este en todo el documento?

Colocando en el preambulo los siguientes comandos. Con sus respectivas distancias y unidades

`\setlenght{\parskip}{  }`

`\setlenght{\parindent}{  }`

Por secuencialización, donde pongamos el comando, los parrafos siguientes resultaran afectados.

_podemos repetir el comando las veces que nosotros deseemos_


## Unidades para medidas en latex

- cm
- mm
- px
- in
- pt
- em (Lo que mide la letra M horizontal)
- ex (Lo que mide la letra x vertical)



## ¿Como podemos modificar el espacio entre parrafos y la sangria de todos los parrafos del documento?

En el __Preambulo__

```latex
% ...

\setlenght{parskip}{8mm}
\setlenght{parindent}{0mm}

\begin{document}
% ...
\end{document}

% ...
```

Esto afectara a todos los parrafos del documento, pero siempre podemos modificar uno solo utilizando la forma de un solo parrafo.

