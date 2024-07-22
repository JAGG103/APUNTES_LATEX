# Partes de una tesis

## ¿En que familias puede dividirse una Tesis?

_book_
- Parte `\part`
- Capitulo `\chapter`
- Sección `\section`
- Subsección `\subsetion`
- Subsubsección `\subsubsection`

_Puede contener capitulos sin contener ninguna parte_


## ¿Que partes contiene una Tesis?

- Portada
- Preámbulo (Se puede disponer del acta de veredicto, agradecimiento, dedicatoria, resumen)
- Índice (Figuras, tablas, codigos, formulas)
- Capítulos
- Bibliografías
- Anexos

## ¿Como podemos construir los elementos del preambulo? ¿Por que?

Utilizando el comando `\chapter*{}` con un asterisco despues del comando y antes de la parte del argumento:

para los agrademientos, dedicatoria y resumén.

Utilizar este formato permite que estos tres ultimos tengan el formato de un capitulo sin ser un capitulo y estar antes del inicio de los mismos.

![](figures\preambulo.png)

