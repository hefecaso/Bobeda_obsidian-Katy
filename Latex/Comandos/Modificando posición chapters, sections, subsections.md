														10-03-2023

>[!cite] Índice: [[Índice LaTex]]

# Modificando posición chapters, sections, subsections

ara centrar el texto de los capítulos (`chapter`), secciones (`section`) y subsecciones (`subsection`) en LaTeX, puedes usar el paquete `titlesec`. Este paquete te permite personalizar el formato de los títulos de las secciones en tu documento.

Para centrar el texto de las secciones, puedes usar la siguiente línea de código en el preámbulo de tu documento:

```Latex
%>>>>>>>> Posición chapters, subsection y section <<<<<<<<<

\usepackage{titlesec}
\titleformat{\chapter}[display]{\centering\bfseries}{\large\chaptername\ \thechapter}{0pt}{\large}
\titleformat{\section}[block]{\centering\bfseries}{\thesection}{1em}{}
\titleformat{\subsection}[block]{\centering\bfseries}{\thesubsection}{1em}{}
```


Aquí se está utilizando el comando `titleformat` para personalizar el formato de los títulos de las secciones, y se está estableciendo el formato centrado para los títulos de los capítulos, secciones y subsecciones.

La primera línea del comando `titleformat` establece la sección que se va a formatear (en este caso, `\chapter`, `\section` y `\subsection`). El segundo argumento especifica el formato de la sección, en este caso, centrado (`\centering`) y en negrita (`\bfseries`).

El tercer argumento especifica el número y nombre de la sección, en este caso, el nombre del capítulo (`\chaptername`) seguido del número de capítulo (`\thechapter`). En las secciones y subsecciones, solo se muestra el número (`\thesection` o `\thesubsection`).

El cuarto argumento es la separación horizontal entre el número y el título de la sección, establecido en 0pt para los capítulos y 1em para las secciones y subsecciones.

Finalmente, el quinto argumento especifica el formato del título de la sección en sí. Para los capítulos y secciones, simplemente se establece en `\large`, mientras que para las subsecciones no se especifica ningún formato adicional.

Con estas líneas de código, deberías poder centrar los títulos de las secciones en tu documento LaTeX.

--------------------------------------------------

En LaTeX, `1em` es una unidad de medida que se utiliza para especificar distancias relativas a la fuente actual. La longitud `1em` es igual al ancho de la letra "M" en la fuente actual.

Entonces, si se especifica una separación horizontal de `1em` entre el número de sección y el título de la sección, se está estableciendo la separación igual a la anchura de la letra "M" en la fuente actual.

La unidad `em` es útil porque se ajusta automáticamente al tamaño de la fuente actual, lo que significa que la separación horizontal se mantendrá proporcional a la fuente, independientemente del tamaño de la fuente que se esté utilizando. Por ejemplo, si cambias el tamaño de la fuente de tu documento, las separaciones horizontales también se ajustarán automáticamente en consecuencia.

En resumen, `1em` es una unidad de medida en LaTeX que se ajusta automáticamente al tamaño de la fuente actual y se utiliza para especificar distancias relativas a la fuente actual.

--------------------------------------------------

# Notas
> [!note]  Notas
> - Nota 1
> - Nota 2

--------------------------------------------------

# Links de referencias obsidian

> [!cite]  Links de referencias obsidian
> - Nota 1
> - Nota 2

--------------------------------------------------

# Links de referencias urls

> [!cite]  Links de referencias obsidian
> - __Título :__ URL
> - __Título :__ URL

--------------------------------------------------

# Etiquetas
> [!info] Etiquetas
> - #LaTex 
> - Etiqueta 2