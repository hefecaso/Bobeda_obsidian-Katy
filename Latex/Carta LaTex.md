Tags: #LaTex 
Created: 04-03-2023 11:46 

--- 

# Carta

Una carta es un documento más informal que puede incluir elementos como el destinatario, el remitente, una fecha, etc. Este es un ejemplo de preámbulo para una carta:

```Latex
\documentclass[12pt]{letter}

\address{Dirección del remitente}
\signature{Firma del remitente}

\begin{document}

\begin{letter}{Destinatario\\Dirección\\Ciudad, Estado}

\opening{Estimado destinatario,}

% Contenido de la carta

\closing{Atentamente,}

\end{letter}

\end{document}
```

--- 

Links: 

--- 

Source: [[Tipos de documentos LaTex]]