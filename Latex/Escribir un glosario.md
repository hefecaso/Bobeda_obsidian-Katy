														12-03-2023

>[!cite] Índice: [[Índice LaTex]]

# Escribir un glosario

Para hacer un glosario en LaTeX, puede utilizar el paquete "glossaries". A continuación, se presenta un ejemplo básico de cómo utilizar este paquete para crear un glosario:

1.  Agregue el paquete "glossaries" en el preámbulo de su documento LaTeX:

```Latex
%>>>>>>>>>>>>>>>> Para la parte de glosarios <<<<<<<<<<<<<<<<
\usepackage{glossaries}
\makeglossaries
```

2.  Cree una entrada en el glosario con el siguiente comando:

```Latex
\newglossaryentry{nombre}{
   name={término},
   description={definición del término}
}
```

Reemplace "nombre" con el nombre que desee dar a la entrada del glosario, "término" con el término que desea definir y "definición del término" con la definición correspondiente.

3.  Agregue la entrada del glosario en el texto utilizando el siguiente comando:

```Latex
\gls{nombre}
```

Esto mostrará el término y la definición en el texto.

4.  Para imprimir el glosario en el documento, agregue el siguiente comando en el lugar donde desea que aparezca:

```Latex
\printglossary
```

Esto imprimirá todas las entradas del glosario en el orden en que se hayan utilizado en el texto.

Para obtener más información sobre cómo personalizar y utilizar el paquete "glossaries", consulte la documentación del paquete.

## Ejemplo

```Latex
\documentclass{article}
\usepackage{glossaries}

\makeglossaries


\newglossaryentry{maths}
{
    name=mathematics,
    description={Mathematics is what mathematicians do}
}

\newglossaryentry{latex}
{
    name=latex,
    description={Is a markup language specially suited for 
scientific documents}
}


\newglossaryentry{formula}
{
    name=formula,
    description={A mathematical expression}
}

\begin{document}

The \Gls{latex} typesetting markup language is specially suitable 
for documents that include \gls{maths}. \Glspl{formula} are rendered 
properly an easily once one gets used to the commands.

\clearpage

\printglossary[title=Special Terms, toctitle=List of terms]

\end{document}
```


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
> - [Escribir un glosario - Overleaf](https://www.overleaf.com/learn/latex/Glossaries)

--------------------------------------------------

# Etiquetas
> [!info] Etiquetas
> - #LaTex 
> - Etiqueta 2