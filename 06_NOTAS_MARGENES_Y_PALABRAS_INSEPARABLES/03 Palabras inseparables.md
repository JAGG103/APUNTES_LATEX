# Palabras inseparables

## ¿Que son las palabras inseparables?

Son palabras las cuales latex no podra separar y debera ajustar el texto a estas.

## ¿Que comando nos permite convertir una palabra a inseparable?

`~\mbox{Palabra inseparable}`

## ¿Como podemos declarar al compilador de latex como separa una palabra?

Existen dos formas de hacerlo:


1. En el preambulo usando el comando `\hyphenation{pa-la-bra}` en su argumento debemos de sapara la palabra con guiones

2. Donde aparezca la palabra en el texto podemos utilizar `\-` : `\-pa\-la\-bra`

