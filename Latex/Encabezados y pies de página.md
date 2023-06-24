														04-08-2022

>[!cite] Índice:[[Índice LaTex]]

# Encabezados y pies de página

> [!important] 
> Solo funciona con el modo **exam**

## Encabezados y pies que afectan a todo el documento

Tanto en los encabezados como en el pie podemos poner texto en la parte izquierda, central o derecha.

Si deseamos el mismo **encabezado** para todo el documento pondremos:

```latex
\header{Texto izquierda}{Texto centro}{Texto derecha}
```

Podemos dejar cualquiera de las tres llaves vacías. Además, de forma alternativa podremos utilizar estas instrucciones que ponemos a continuación, que hacen exactamente lo mismo aunque tratando por separado los tres espacios izquierdo, central y derecho:

```latex
\lhead{Texto izquierdo}
```
```latex
\chead{Texto central}
```
```latex
\rhead{Texto derecho}
```

Exactamente lo mismo se aplica al **pie** con:

```latex
\footer{Texto izquierda}{Texto centro}{Texto derecha}
```

y

```latex
\lfoot{Texto izquierdo}
```
```latex
\cfoot{Texto central}
```
```latex
\rfoot{Texto derecho}
```

Si queremos una línea horizontal bajo el encabezado pondremos `\headrule` y en el pie `\footrule`.

Veamos un ejemplo:

```latex
\documentclass[11pt,a4paper,addpoints]{exam}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage[spanish]{babel}
\usepackage[left=2.00cm, right=2.00cm, top=2.00cm, bottom=2.00cm]{geometry}

\begin{document}

\header{Agosto de 2020}{}{Bachillerato}
\footer{Tema 1}{Página\ \thepage\ de \numpages}{Encabezados y pies}
\headrule
\footrule

 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet risus ac turpis condimentum tincidunt. Ut scelerisque dolor ac purus aliquam, quis tincidunt metus ultricies. Sed velit augue, ullamcorper sed laoreet sit amet, ultrices eget felis.
\newpage
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet risus ac turpis condimentum tincidunt. Ut scelerisque dolor ac purus aliquam, quis tincidunt metus ultricies. Sed velit augue, ullamcorper sed laoreet sit amet, ultrices eget felis.
\end{document}
```

Copy

El encabezado se ve así:

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-13.png)

Encabezado, la parte central se dejó vacía.

Y el pie:

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-1-2.png)

El número de página se consigue con \thepage y el número total con \numpages, esto último requiere una doble compilación para que las cuente correctamente.

## Encabezados y pies de la primera página y del resto

Podemos diferenciar la primera página del resto de páginas. Para poner encabezados y pies en la primera página usaremos:

-   `\firstpageheader{Izquierda}{Centro}{Derecha}` para el encabezado de la primera página.
-   `\firstpagefooter{Izquierda}{Centro}{Derecha}` para el pie de la primera página.

Para el resto de las páginas, es decir, a partir de la segunda:

-   `\runningheader{Izquierda}{Centro}{Derecha}` para el encabezado de las páginas siguientes a la primera.
-   `\runningfooter{Izquierda}{Centro}{Derecha}` para el pie de las páginas siguientes a la primera.

Una forma alternativa de indicar esto mismo es indicar entre **corchetes** el contenido de la primera página y entre **llaves** el de las siguientes:

Encabezados

| Posición  | Encabezados              | Pies                     |
| --------- | ------------------------ | ------------------------ |
| Izquierda | \lhead[Pag1]{Siguientes} | \lfoot[Pag1]{Siguientes} |
| Centro    | \chead[Pag1]{Siguientes} | \cfoot[Pag1]{Siguientes} |
| Derecha   | \rhead[Pag1]{Siguientes} | \rfoot[Pag1]{Siguientes} | 

Asignación de encabezados y pies a la primera página o a las siguientes en diferentes posiciones.

Por ejemplo, para poner el texto: «Examen» en la parte izquierda del encabezado de la primera página y «Nombre:» en la misma posición del resto de páginas pondríamos: `\lhead[Examen]{Nombre:}`

## Líneas horizontales

Para obtener líneas de separación de los encabezados y pies podemos usar lo siguiente:

| Instrucción        | Efecto                                            |
| ------------------ | ------------------------------------------------- |
| \headrule          | Encabezados: Líneas en todas las páginas.         |
| \footrule          | Pies: Líneas en todas las páginas.                |
| \firstpageheadrule | Encabezados: Línea en la primera página.          |
| \firstpagefootrule | Pies: Línea en la primera página   .              |
| \runningheadrule   | Encabezados: Líneas a partir de la segunda página |
| \runningfootrule   | Pies: Líneas a partir de la segunda página        | 

## Ejemplo

Veamos un ejemplo donde mezclamos un poco de todo lo anterior.

```latex
\documentclass[11pt,a4paper,addpoints]{exam}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage[spanish]{babel}
\usepackage[left=2.00cm, right=2.00cm, top=2.00cm, bottom=2.00cm]{geometry}

\begin{document}

\lhead[Lorem ipsum]{Agosto 2020}
\chead[2020]{Lorem ipsum}
\rhead[]{Encabezados}
\runningfooter{Tema 1}{Página\ \thepage\ de \numpages}{Encabezados y pies}
\headrule
\runningfootrule

 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet risus ac turpis condimentum tincidunt. Ut scelerisque dolor ac purus aliquam, quis tincidunt metus ultricies. Sed velit augue, ullamcorper sed laoreet sit amet, ultrices eget felis.
\newpage
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet risus ac turpis condimentum tincidunt. Ut scelerisque dolor ac purus aliquam, quis tincidunt metus ultricies. Sed velit augue, ullamcorper sed laoreet sit amet, ultrices eget felis.
\end{document}
```

Copy

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-14.png)

Encabezado de la primera página. No se ha definido ningún tipo de pie para esta página.

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-1-3.png)

Encabezado de la segunda página y siguientes.

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-2-2.png)

Pie de página de la segunda página y siguientes.

## Páginas pares e impares

Muchas veces es útil diferenciar las páginas pares de las impares. Esto se puede hacer con la orden `\oddeven{Texto si página impar}{Texto si página par}`. Introduciendo esta instrucción en un encabezado o pie podemos hacer que se imprima un texto u otro según la página en la que estemos sea impar o par. Esta instrucción **solo funciona correctamente en los encabezados y pies**.

Veamos un ejemplo donde no se imprime encabezado en la primera página y en las impares se pide el nombre del alumno, mientras que en las pares se escribe el nombre del examen.

```latex
\documentclass[11pt,a4paper,addpoints]{exam}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage[spanish]{babel}
\usepackage[left=2.00cm, right=2.00cm, top=2.00cm, bottom=2.00cm]{geometry}

\begin{document}

\lhead[]{ \oddeven{Nombre:}{Examen de Biología}}

\runningheadrule 

Texto página 1
\newpage
Texto página 2
\newpage
Texto página 3
\newpage
Texto página 4

\end{document}
```

Copy

## Diferenciar la última página

De forma similar a la instrucción anterior existe `\iflastpage` que permite escribir texto específico en el encabezado y pie de la última página. El funcionamiento es el siguiente: `\iflastpage{texto si es la última}{texto si no lo es}`. El siguiente ejemplo imprime el número de páginas en el pie de todas las páginas excepto en la ultima donde imprime «Fin del examen»:

```latex
\cfoot{\iflastpage{Fin del examen}{Página\ \thepage\ de\ \numpages}}
\footrule
```

Copy

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-3-1.png)

Pie de una de las páginas que no es la última.

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-4-1.png)

Pie de la última página.

## Encabezados y pies multilínea

Para que el texto de un encabezado o pie ocupe más de una línea bastará con añadir una doble barra invertida para crear un salto de línea: `\\`. Si necesitamos más espacio usaremos las instrucciones:

-   `\extraheadheight{xcm}` Espacio extra para el encabezado.
-   `\extrafootheight{xcm}` Espacio extra para el pie.

Veamos un ejemplo con un encabezado con dos líneas en todas las páginas al que damos un espacio extra de 0.25cm.

```latex
\documentclass[11pt,a4paper,addpoints]{exam}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage[spanish]{babel}
\usepackage[left=2.00cm, right=2.00cm, top=2.00cm, bottom=2.00cm]{geometry}

\begin{document}

\extraheadheight{0.25cm}
\header{}{La célula\\Examen de Ciencias Naturales}{}
\headrule

Texto

\end{document}
```

Copy

![](https://educacion.bilateria.org/wp-content/uploads/2020/08/captura-5-1.png)

Encabezado con dos líneas, se consigue poniendo: \\

## Numeración de las páginas

Podemos poner el número de página en cualquier lugar de los encabezados y pies escribiendo `\thepage`. El número total de páginas se consigue con `\numpages`. Si utilizamos esta última instrucción será necesario hacer una doble compilación para que se calcule correctamente el número de páginas.

Aunque en la documentación oficial no habla de esto, se ha visto que si escribimos: `Página \thepage de \numpages` en lugar de obtener algo así como «Página 3 de 5» se obtiene «Página3de5», sin espacios, por lo que hay que forzar los espacios con la barra invertida: `\` , es decir: `Página\ \thepage\ de\ \numpages`.

## ¿Algo más sobre encabezados y pies?

Sí, todavía quedan los comandos que detectan si una pregunta continúa desde la página anterior y quizás deseamos indicarlo en el encabezado (o pie) con algo así como «Continuación de la pregunta 7». No obstante, esto lo dejamos para otra ocasión, si deseas averiguar cómo se hace consulta la sección 11.9 del documento [Using the exam document class](http://www-math.mit.edu/~psh/exam/examdoc.pdf).


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
> - __Referencia:__ https://educacion.bilateria.org/encabezados-y-pies-de-la-clase-exam-en-latex#:~:text=Podemos%20diferenciar%20la%20primera%20p%C3%A1gina,pie%20de%20la%20primera%20p%C3%A1gina.
> - __Título :__ URL

--------------------------------------------------

# Etiquetas
> [!info] Etiquetas
> - #LaTex 
> - Etiqueta 2