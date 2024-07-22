# Númeración de páginas

## ¿Como podemos dividir los elementos de la tesis considerando dos grandes grupos y le enumeración?

```latex
\documentclass{book}
\usepackage[uft8]{inputenc}
\usepackage[spanish]{babel}
\title{Thesis}
\author{Jhonatan}
\date{\today}

\begin{document}
\maketitle
\newpage
\thispagestyle{empty}


%----------------------[GROUP ONE]
\chapter*{Resumen}
\chapter*{Agradecimientos}
\chapter*{}

%----------------------[GROUP TWO]
\chapter{Introducción}
\chapter{Marco Teórico}

\end{document}
```

## ¿Como se deben de enumerar los dos grupos?

El grupo 1 debe de utilizar enumeración __ROMANA__

El grupo 2 debe de utilizar enumeración __ARABIGA__

```latex
\chapter*{Resumen}
\pagenumbering{Roman}
\setcounter{page}{1}

\chapter{Introducción}
\pagenumbering{arabic}
\setcounter{page}{1}
```

## ¿Que comando nos permite configurar la enumeración?

```latex
\pagenumbering{Roman} % \pagenumering{arabic}
\setcounter{page}{1}
```

Justo en el capitulo donde queremos utilizar esta enumeración.