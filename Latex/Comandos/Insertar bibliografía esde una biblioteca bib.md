														24-06-2022

>[!cite] Índice: [[Índice LaTex]]

# Insertar bibliografía esde una biblioteca bib

```Latex
\usepackage{apacite}

  

%%%%%%%%%%%%%%%%%%%%%

%	Bibliografías	%

%%%%%%%%%%%%%%%%%%%%%

\clearpage

%Primero darle a F11, luego a F6 y por último compilamos, así veremos la bibliografía, esto cada vez que hagamos una citación en nuestro documento.
  

\bibliographystyle{apacite}

\nocite{*} %Descomentar para que genere la bibliografía sin citar

%\cite{Einstein} Para sitar al final del parrafo citado.

%\cite[p.10]{Einstein} Para citar al final del parrafo citado con página.

%\nocite{Einstein} Para mostrar en referencias sin citar.

\bibliography{Nombre_del_archivo_bib}


%https://dle.rae.es/mililitro
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