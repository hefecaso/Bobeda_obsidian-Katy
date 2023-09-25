														27-08-2023

>[!cite] Índice: [[Índice LaTex]]

# Colocar un índice dentro de otro índice

El comando `\addtocontents` en LaTeX se utiliza para agregar contenido personalizado a los archivos de índice y otros archivos generados automáticamente, como la tabla de contenidos, la lista de figuras y la lista de tablas. Puedes utilizarlo para incluir información adicional en estos archivos de índice, lo que te permite personalizar la forma en que se muestran ciertos elementos en los índices. 

La sintaxis básica del comando `\addtocontents` es la siguiente:

```latex
\addtocontents{<archivo>}{<contenido>}
```

Donde:
- `<archivo>` es el nombre del archivo de índice al que deseas agregar contenido (por ejemplo, `toc` para la tabla de contenidos, `lof` para la lista de figuras, `lot` para la lista de tablas, etc.).

>[!note]Nota
>Esto quiere decir que lo que tenga **toc**, irá al índice general, **lof** a la tabla de figuras y **lot** se mostrará en la lista de tablas.

- `<contenido>` es el contenido que deseas agregar al archivo de índice.

Por ejemplo, si deseas agregar una entrada personalizada a la tabla de contenidos, puedes hacerlo de la siguiente manera:

```latex
\addtocontents{toc}{\protect\contentsline{chapter}{Mi Entrada Personalizada}{3}}
```

En este caso, el comando agrega una entrada para un capítulo llamado "Mi Entrada Personalizada" en el archivo `toc` (tabla de contenidos) y especifica el número de página donde aparece esa entrada (en este caso, la página 3).

Ten en cuenta que `\protect` se utiliza aquí para asegurarse de que los comandos internos sean procesados correctamente y no generen errores.

Recuerda que después de utilizar `\addtocontents`, es posible que necesites compilar el documento varias veces para que los cambios en los archivos de índice se reflejen correctamente en el documento final.

--------------------------------------------------

Colocamos lo siguiente en el preámbulo:

```Latex
%>>>>>>>>>>>>>>>>> Comando índices <<<<<<<<<<<<<<<<<<<<<<
\usepackage{tocloft} % Necesario para personalizar la apariencia del índice

\renewcommand{\cftchapdotsep}{\cftdotsep} % Puntos de relleno para los capítulos en el índice
```

Y lo siguiente dentro del documento:

```Latex
\documentclass{report}

\begin{document}

%%%%%%%%%%%%%
%   Índices %
%%%%%%%%%%%%%

% Cambiar el contador de página a números romanos temporalmente, número de páginas.
\pagenumbering{roman}

% Índice general
\newpage
\tableofcontents
\clearpage


% Agregar entrada de la lista de tablas al índice con números romanos

% Lista de tablas
\phantomsection % Coloca el punto de referencia al cual llevará el enlace
\addcontentsline{toc}{chapter}{ÍNDICE DE TABLAS}
\listoftables
\clearpage

% Lista de figuras
%\newpage
\phantomsection % Coloca el punto de referencia al cual llevará el enlace
\addcontentsline{toc}{chapter}{ÍNDICE DE ILUSTRACIÓNES}
\listoffigures
\clearpage


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%   Capítulos de la tesis   %
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

% Restaurar el contador de página a números arábigos, número de páginas.
\pagenumbering{arabic}

\chapter{Introducción}
Contenido introductorio.

\chapter{Desarrollo}
Contenido de desarrollo.

\end{document}
```

En este ejemplo, he utilizado `\addcontentsline` para agregar entradas personalizadas en el índice para la tabla de contenidos, la lista de tablas y la lista de figuras. Puedes cambiar los nombres "Índice General", "Lista de Tablas" y "Lista de Figuras" a lo que desees. Esto asegurará que aparezcan los nombres personalizados en el índice en lugar de los nombres predeterminados.

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
> - [Título](link)
> - [Título](link)

--------------------------------------------------

> [!info] Etiquetas
> - #LaTex 
> - Etiqueta 2