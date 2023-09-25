Tags: #LaTex 
Created: 10-03-2023 10:34 

--- 

# Plantilla para una tesis en formato article

```Latex
\documentclass[12pt,oneside]{article} % Clase del documento y opciones

% Paquetes requeridos para la plantilla
\usepackage[spanish,es-tabla]{babel} % Idioma y configuración para tablas
\usepackage[utf8]{inputenc} % Codificación de caracteres
\usepackage[T1]{fontenc} % Codificación de fuentes
\usepackage{graphicx} % Manejo de gráficos
\usepackage{setspace} % Espaciado personalizado
\usepackage{amsmath, amssymb, amsfonts} % Símbolos matemáticos y fuentes
\usepackage{hyperref} % Configuración de enlaces
\usepackage{enumitem} % Personalización de listas
\usepackage{cite} % Citas bibliográficas
\usepackage{caption} % Personalización de leyendas
\usepackage{subcaption} % Manejo de subfiguras

% Márgenes recomendados para una tesis
\usepackage[top=2.5cm,bottom=2.5cm,left=3cm,right=2cm]{geometry}

% Estilo de fuente recomendado para una tesis
\usepackage{times}

% Configuración de encabezados y pies de página
\usepackage{fancyhdr} % Manejo de encabezados y pies de página
\pagestyle{fancy} % Estilo de página personalizado
\fancyhf{} % Elimina encabezados y pies de página previos
\renewcommand{\headrulewidth}{0.5pt} % Grosor de la línea del encabezado
\renewcommand{\footrulewidth}{0pt} % Grosor de la línea del pie de página
\fancyhead[LE,RO]{\thepage} % Números de página en el encabezado
\fancyhead[RE]{\nouppercase{\leftmark}} % Capítulo actual en el encabezado derecho
\fancyhead[LO]{\nouppercase{\rightmark}} % Sección actual en el encabezado izquierdo

% Configuración de estilo de títulos de secciones
\usepackage{titlesec} % Personalización de títulos
\titleformat{\chapter}[display] % Formato de capítulos
{\normalfont\bfseries\filcenter}{\MakeUppercase{\chaptertitlename}\ \thechapter}{0pt}{\Large} % Formato de título de capítulo
\titlespacing*{\chapter}{0pt}{-30pt}{20pt} % Espaciado personalizado de capítulos

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%   Inicio del documento    %
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\begin{document}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%	Cambiando nombre de referencias a bibliografía	%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Cambiando el nombre de los cuadros y referencias a:
%Tabla y bibliografía

%Cambiando Referencia por Bibliografía
\renewcommand{\refname}{Bibliografía}
%Cambiando Cuadro por tabla
%\renewcommand{\tablename}{Tabla}
%Cambiando Cuadro por tabla
%\renewcommand{\figurename}{Figura}
%Cambiando enumeración arábica a romana en figuras
%\renewcommand{\thefigure}{\roman{figure}}
%Cambiando enumeración arábica a romana en tablas
%\renewcommand{\thetable}{\roman{table}}

%\renewcommand{\thechapter}{}

% Portada
\input{portada.tex} % Archivo para portada

% Página de resumen
\input{resumen.tex} % Archivo para resumen

% Dedicatoria
\input{dedicatoria.tex} % Archivo para dedicatoria

% Agradecimientos
\input{agradecimientos.tex} % Archivo para agradecimientos

% Tabla de contenidos
\tableofcontents % Índice de contenidos

% Lista de tablas

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%   Capítulos de la tesis   %
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\input{capitulo1.tex} 
\input{capitulo2.tex} 
\input{capitulo3.tex} 
\input{capitulo4.tex} 
\input{capitulo5.tex} 

% Referencias bibliográficas 
\bibliographystyle{apalike} 
\bibliography{bibliografia.bib} 

\end{document}
```

Esta plantilla incluye los siguientes elementos:

-   Paquetes requeridos para la plantilla
-   Márgenes y estilo de fuente recomendados para una tesis
-   Configuración de encabezados y pies de página
-   Configuración de estilo de títulos de secciones
-   Configuración de estilo de tablas y figuras
-   Portada, resumen, dedicatoria, agradecimientos, tabla de contenidos, lista de tablas, lista de figuras
-   Capítulos de la tesis
-   Referencias bibliográficas

Ten en cuenta que esta plantilla es solo una sugerencia y que puedes personalizarla según tus necesidades y preferencias.

--------------------------------------------------

El comando `\input` en LaTeX se utiliza para insertar el contenido de un archivo externo en el documento actual. Esto puede ser útil cuando tienes una tesis, por ejemplo, con muchos capítulos o secciones, y prefieres tener cada uno en un archivo separado para facilitar su edición y organización.

El comando `\input` se utiliza de la siguiente manera:

```Latex
\input{nombre-del-archivo}
```

donde `nombre-del-archivo` es el nombre del archivo que se desea insertar. La extensión del archivo no es necesaria, ya que LaTeX busca por defecto los archivos con las extensiones `.tex`, `.sty` y `.cls`.

Por ejemplo, si tienes un archivo llamado `capitulo1.tex` con el contenido de tu primer capítulo, puedes insertarlo en tu documento principal con el siguiente comando:

```Latex
\input{capitulo1}
```

Al compilar el documento principal, LaTeX buscará el archivo `capitulo1.tex` en la misma carpeta y lo incluirá en el documento en el lugar donde se encuentra el comando `\input`.

El uso de `\input` permite una mejor organización del código y una mayor modularidad del documento, lo que puede facilitar su edición y mantenimiento en el largo plazo.

--- 

Links: 

--- 

Source: 
[[Tipos de documentos LaTex]]