														09-02-2023

>[!cite] Índice: [[Índice LaTex]]

# Modificando el nombre de partes del documento

```Latex
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%	Cambiando nombre de referencias a bibliografía	%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Cambiando el nombre de los cuadros y referencias a:
%Tabla y bibliografía

%Cambiando Referencia por Bibliografía
\renewcommand{\refname}{Bibliografía}
%Cambiando Cuadro por tabla
%\renewcommand{\tablename}{Tabla}
%Cambiando enumeración arábica a romana en figuras
%\renewcommand{\thefigure}{\roman{figure}}
%Cambiando enumeración arábica a romana en tablas
%\renewcommand{\thetable}{\roman{table}}

%\renewcommand{\thechapter}{}
```

Esto se coloca entre \begin{document} y \end{document}

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