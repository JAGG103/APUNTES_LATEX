# Perfiles

## ¿Que son los perfiles? 

Es una caracteristica extra a las fuentes que nos permiten resaltar o diferenciar cierta parte del texto

## ¿Que tipos de perfiles nos permite utilizar latex?

- Perfil recto `\textup{text}`

- Perfil italico `\textit{text}`

- Perfil inclinado `\textsl{text}`

- Perfil versalita `\textsc{text}`

## ¿Cuales son las 3 formas de modificar los perfiles?

1. Comando + Argumento

```latex
\textup{text} % 
\textit{text} 
\textsl{text} 
\textsc{text}
```

2. Bloque + Orden

```latex
{
\upshape % \itshape \slshape \scshape
text
}
```

3. Entorno

```latex
\begin{scshape}
text
\end{scshape}
```