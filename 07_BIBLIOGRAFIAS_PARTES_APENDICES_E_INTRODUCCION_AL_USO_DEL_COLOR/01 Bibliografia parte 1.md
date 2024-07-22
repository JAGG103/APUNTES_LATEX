# Bibliografia parte 1

## Para una mejor organización del documento ¿Que se recomienda hacer con las partes?

Se recomienda divir el documetos en carpetas las cuales contendran alguna parte especifica del documento:

PORTADA
	portada.text
PREAMBULO
	dedicatoria.tex
	agradecimientos.tex
	resumen.tex
CAPITULOS
	capitulo 1
	capitulo 2
main.tex
bibliografia.bib

## ¿Como podemos hacer uso de bibliografias?

Debemos crear en el espacio del proyecto un archivo .bib

El cúal contendra las referencias en un formato especifico que latex utiliza.

## ¿Que significan las diferentes identaciones en el formato de las bibliografias?

Los items identados mas a la izquierda son __obligatorios__ y los mas a la derecha son __opcionales__

_Si no provee algun item latex podra construir la bibliografia_

## Si hay mas de un autor para una referencia como se deben de colocar?

Con la primera letra del nombre seguida por el apellido separados por el operador __and__

`author = {I. Guerrero and I. Guerrero and I. Guerrero}`

## ¿Cuáles son los tipos de referencias bibliograficas que tiene latex?

Las bibliograficas deben de guardarse en un archivo .bib respetando la sintaxis siguiente.

1. Articulo : revista de prublicación periodica

```latex
@article{,
	author={},
	title={},
	journal={},
	year={},
		volumen={},
		number={},
		pages={},
		month={},
		note={}
}
```

2. Libros (editorial conocida)

```latex
@book{,
	author={},
	editor={},
	title={},
	publisher={},
	year={},
		volumen={},
		number={},
		series={},
		address={},
		edition={},
		month={},
		note={}
}
```


3. Libros (No publicados por una editorial)

```latex
@booklet{,
	title={},
		author={},
		howpublished={},
		address={},
		month={},
		year={},
		note={}
}
```


4. Parte de libros (Capitulos, secciones o rango de paginas)

```latex
@inbook{,
	author={},
	editor={},
	title={},
	chapter={},
	pages={},
	publisher={},
	year={},
		volume={}, 
		number={},
		series={},
		type={},
		address={},
		edition={},
		month={},
		note={}
}

```

5. Coleccion (libros que sean partes de una colección)

```latex
@incollection{,
	author={},
	title={},
	booktitle={},
	publicher={},
	year={},
		edition={},
		volume={},
		number={},
		series={},
		tupe={},
		chapter={},
		pages={},
		eddress={},
		edition={},
		month={mayo}
}
```

6. parte de comunicaciones a congresos

```latex
@inproceedings{,
	author={},
	title={},
	booktitle={},
	year={},
		editor={},
		volumen={},
		number={},
		series={},
		pages={},
		address={},
		month={},
		organization={},
		publisher={},
		note={}
}
```


7. Manual (Documentación tecnica)

```latex
@manual{bib7,
		author={},
		organization={},
		address={},
		edition={},
		month={},
		year={},
		note={}
}
```

8. 	Tesis de maestria 

```latex
@mastersthesis{,
	autor={},
	title={},
	school={},
	year={},
		type={},
		address={},
		month={},
		note={}
}
```

9. Material variado

```latex
@misc{bib9,
		author={},
		title={},
		howpublished={},
		month={},
		year={},
		note={}
}
```

10. Tesis doctorales

```latex
@phdthesis{,
	author={},
	title={},
	school={},
	year={},
		type={},
		address={},
		month={},
		note={}
}
```

11. Comunicaciones a congresos

```latex
@proceedings{,
	title={},
	year={},
		editor={},
		volume={},
		number={},
		series={},
		address={},
		publicher={},
		note={}
}
```

12. Informes publicados por alguna institución

```latex
@techreport{,
	author={},
	title={},
	intitution={},
	year={},
		type={},
		number={},
		address={},
		monthe={},
		note={}
}
```

13. Documentos no publicados actualmente

```latex
@unpublished{,
	author={},
	title={},
	note={},
		month={},
		year={}
}
```


