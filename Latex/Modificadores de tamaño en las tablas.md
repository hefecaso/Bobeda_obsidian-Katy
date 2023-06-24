														31-08-2022

>[!cite] Índice: [[Índice LaTex]]

# Modificadores de tamaño en las tablas

```latex
\usepackage{array}
```

Para dar un formato al entorno `tabular`, tenemos que decir a LaTeX cuántas columnas necesitaremos y cómo deben ser alineadas. Esto se hace con un argumento obligatorio – a menudo llamado preámbulo de la tabla – del entorno `tabular`, en el que se especifican las columnas usando nombres de un sólo carácter, llamados identificadores de preámbulo. Los tipos de columna disponibles son:

| Tipo            | Descripción                                                                                                                                                                  |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| l               | Columna justificada a la izquierda.                                                                                                                                          |
| c               | Columna centrada.                                                                                                                                                            |
| r               | Columna justificada a la derecha.                                                                                                                                            |
| p{width}        | Columna con un ancho **width** fijo; el texto sera automáticamente ajustado a la línea y justificado.                                                                        |
| m{width}        | Como **p**, pero centrado verticalmente con respecto al resto del texto de la misma fila.                                                                                    |
| b{width}        | Como **p**, pero ajustado verticalmente a la parte baja de la celda.                                                                                                         |
| w{align}{width} | Imprime el contenido con un ancho **width** fijo, sobreimprimiendo si el texto es muy largo. Puede elegir el justificado horizontal **align** usando **l**, **c**, or **r**. | 
| W{align}{width} | Como **w**, pero dando lugar a un mensaje de alerta «overfull box warning» si el texto es demasiado grande.                                                                    |

Además, otros identificadores de preámbulo adicionales están disponibles, estos no son para definir columnas pero pueden serle de gran utilidad igualmente:

| Tipo            | Descripción                                                                                                                                                          |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| \*{num}{string} | Repite **string** un número **num** de veces en el preámbulo. De esta forma puede definir múltiples columnas idénticas.                                             |
| >{decl}         | Coloca **decl** antes del contenido de cada celda de la columna que sigue al identificador (útil, por ejemplo, para una fuente de letra diferente en esta columna). |
| <{decl}         | Coloca **decl** después del contenido de cada celda de la columna previa a la declaración.                                                                          |
| \|              | Añade una línea vertical.                                                                                                                                           |
| @{decl}         | Reemplaza el espacio existente entre dos columnas por **decl**.                                                                                                     |
| !{decl}         | Añade **decl** en el centro del espacio existente.                                                                                                                  | 


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
> - #LaTex 
> - Etiqueta 2