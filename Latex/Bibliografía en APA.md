														22-01-2023

>[!cite] Índice: [[Índice LaTex]]

# Bibliografía en APA

```latex
\documentclass{article}
\usepackage[canadian]{babel}
\usepackage{csquotes}
\usepackage[style=apa,backend=biber]{biblatex}
\DeclareLanguageMapping{canadian}{canadian-apa}
\addbibresource{test.bib}
\begin{document}
This statement is true \parencite[5-8]{Ref}.
\printbibliography
\end{document}
```

Entonces en el preambulo colocaremos:

```LaTex
\usepackage[style=apa,backend=biber]{biblatex}
\DeclareLanguageMapping{canadian}{canadian-apa}
\addbibresource{test.bib}
```

Si la bibliografía no se imprime, probar la siguiente configuración en el preambulo:

```Latex
\usepackage[style=apa,backend=bibtex]{biblatex}
```

en donde *"style=apa"* puede ser cambiado por cualquier otro estilo.

--------------------------------------------------

Dentro del documento para poder imprimir la bibliografía colocaremos:

```LaTex
%%%%%%%%%%%%%%%%%%%%% 
%   Bibliografías   % 
%%%%%%%%%%%%%%%%%%%%% 

\clearpage 
%Primero darle a F11, luego a F6 y por último compilamos, así veremos la bibliografía, esto cada vez que hagamos una citación en nuestro documento. 

\nocite{*} 
%Descomentar para que genere la bibliografía sin citar 

%\cite{Einstein} 
%Para sitar al final del parrafo citado. 

%\cite[p.10]{Einstein} Para citar al final del parrafo citado con página. 

%\nocite{Einstein} 
%Para mostrar en referencias sin citar. 

\printbibliography

```

Otra forma de imprimir la bibliografía es:

```Latex
\addbibresource{nombre_archivo.bib}
```


# Otros formatos de bibliografía

## Configuración para APA 6ta edición

Se debe de colocar en el preámbulo:

```Latex
\usepackage[style=apa,backend=biber]{biblatex}
```

## Configuración para APA 7ta edición

Se debe de colocar en el preámbulo:

```Latex
\usepackage[style=apa7,backend=biber]{biblatex}
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
> - __Título :__ URL
> - __Título :__ URL

--------------------------------------------------

# Etiquetas
> [!info] Etiquetas
> - `rir:FileText` #LaTex
> - Etiqueta 2