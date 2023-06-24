														09-02-2023

>[!cite] Índice: [[Índice LaTex]]

# Modificar diseño de chapters y sections

Configuración para modo book, chapter:

```Latex
\usepackage{titlesec, blindtext, color}

\definecolor{gray75}{gray}{0.75}

\newcommand{\hsp}{\hspace{20pt}}

\titleformat{\chapter}[hang]{\Huge\bfseries}{\thechapter\hsp\textcolor{gray75}{|}\hsp}{0pt}{\Huge\bfseries}
```

Configuración para modo article, Capítulos:

```Latex
\usepackage{titlesec, blindtext, color}

\definecolor{gray75}{gray}{0.75}

\newcommand{\hsp}{\hspace{20pt}}

\titleformat{\section}[hang]{\Huge\bfseries}{\thesection\hsp\textcolor{gray75}{|}\hsp}{0pt}{\Huge\bfseries}
```

Todo va afuera del  \begin{document} y \end{document}

--------------------------------------------------

# Notas
> [!note]  Notas
> - Nota 1
> - Nota 2

--------------------------------------------------

# Links de referencias obsidian

> [!cite]  Links de referencias obsidian
> - [Link 1](https://texblog.org/2012/07/03/fancy-latex-chapter-styles/)

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