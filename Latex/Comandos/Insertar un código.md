														24-06-2022

>[!cite] Índice: [[Índice LaTex]]

# Insertar un código V1

## Opción 1

```Latex
\documentclass{article}

\usepackage{minted}

\begin{document}

  

%Para incertar el código utilizamos:

  

\begin{minted}{python}

import numpy as np

def incmatrix(genl1,genl2):

    m = len(genl1)

    n = len(genl2)

    M = None to become the incidence matrix

    VT = np.zeros((n*m,1), int)  dummy variable

    compute the bitwise xor matrix

    M1 = bitxormatrix(genl1)

    M2 = np.triu(bitxormatrix(genl2),1) 

  

    for i in range(m-1):

        for j in range(i+1, m):

            [r,c] = np.where(M2 == M1[i,j])

            for k in range(len(r)):

                VT[(i)*n + r[k]] = 1;

                VT[(i)*n + c[k]] = 1;

                VT[(j)*n + r[k]] = 1;

                VT[(j)*n + c[k]] = 1;

                if M is None:

                    M = np.copy(VT)

                else:

                    M = np.concatenate((M, VT), 1)

                VT = np.zeros((n*m,1), int)

    return M

\end{minted}

\end{document}

  

%Otra forma de insertar el código, directo del programa es usando:

  

\inputminted{python}{Ejemplo.py}
```

## Opción 2

```Latex
\begin{verbatim}

  

Escribes tu código aquí­

  

\end{verbatim}
```

## Opción 3


```Latex
\usepackage{listings}

  

\lstset{language=C, breaklines=true, basicstyle=\footnotesize}

\begin{lstlisting}[frame=single]

include <stdio.h>

include <stdlib.h>

// programa muy positivo

  

void main{

  system("clear");

  printf("Hola mundo!\n");

}

\end{lstlisting}
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