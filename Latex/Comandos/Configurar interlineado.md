														25-02-2023

>[!cite] Índice: [[Índice LaTex]]

# Configurar interlineado

El documento [[Configuración para cualquier documento LaTex]] ya incluye una opción para cambiar el interlineado, línea #16 del documento de obsidian. Pero exite otra forma.

Para establecer el interlineado múltiple de 0.9 en LaTeX, puedes usar el paquete setspace. Este paquete te permite modificar el espaciado entre líneas de tu documento. Para establecer el interlineado múltiple de 0.9, sigue estos pasos:

1.  Añade la siguiente línea al preámbulo de tu documento LaTeX:

```Latex
\usepackage{setspace}
```

2.  Luego, debes establecer el interlineado múltiple de 0.9 utilizando el siguiente comando:

```Latex
\setstretch{0.9}
```

3.  Si quieres que el interlineado se aplique a todo el documento, coloca el comando en el preámbulo. Si solo quieres aplicarlo a un bloque de texto, colócalo antes del texto que deseas ajustar y luego vuelve a establecer el interlineado normal después del texto. Por ejemplo:

```Latex
\setstretch{0.9}

Este es el texto al que se le aplicará el interlineado múltiple de 0.9. 

\setstretch{1.0} 

Este es el texto que volverá al interlineado normal.
```

De esta manera, el interlineado múltiple se ajustará a 0.9 en el bloque de texto especificado y volverá a 1.0 después del bloque.

Espero que esto te ayude a establecer el interlineado múltiple en tu documento LaTeX.

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
> `rir:FileText` #LaTex
> - Etiqueta 2