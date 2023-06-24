Tags: #LaTex 
Created: 04-03-2023 11:39 

--- 

# Tesis o disertación

Una tesis o disertación suele tener una estructura más compleja que un artículo científico, y puede incluir elementos como una página de título, resumen, índice de contenidos, etc. Este es un ejemplo de preámbulo para una tesis o disertación:

```Latex
\documentclass[12pt]{report}

\usepackage{cite}
\usepackage{graphicx}
\usepackage{appendix}

\begin{document}

\include{portada}

\pagenumbering{roman}

\include{resumen}

\tableofcontents
\listoffigures
\listoftables

\clearpage
\pagenumbering{arabic}

\include{capitulo1}
\include{capitulo2}
% Etc.

\appendix
\include{apendiceA}
\include{apendiceB}
% Etc.

\section{Título} 
% Contenido del título 
\subsection{Subtítulo 1}

\bibliographystyle{plain}
\bibliography{bibliografia}

\end{document}

```

Las partes que dicen \include{Documento}, normalmente son extracciónes de otro documento LaTex, en este caso Documento.tex, unificandolos en uno sólo.

Ver ejemplo que se encuentra en los links, en el ejemplo tenemos un documento llamado **"Caratula.tex"**. En el documento principal lo encontramos en la línea **número 127**.

Esto último se puede incluir en cualquier tipo de documento.

--- 

Links: 

[Ver ejemplo dando click aquí.](https://es.overleaf.com/read/nmyxwdnrgfcg)

--- 

Source: [[Tipos de documentos LaTex]]