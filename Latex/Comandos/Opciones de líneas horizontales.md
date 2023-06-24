														23-09-2022

>[!cite] Índice: [[Índice LaTex]]

# Opciones de líneas horizontales

### \hline

```Latex
\hline
```

El comando "\hline" es la más simple de las opciones de línea horizontal en LaTeX y, la mayoría de las veces, es la que deseas. Simplemente traza una línea horizontal entre los apartados que procedan y la sigue cuando el documento es renderizado. Esto también significa que, por supuesto, si "\hline" se utiliza a la mitad del párrafo, entonces forzará un salto en los párrafos.

### \rule

```Latex
\rule
```

El comando "\rule{length}{thickness}" proporciona un poco más de energía que la normal "\hline". En primer lugar, la regla no forza un salto entre párrafos: es aceptable el uso de una regla en medio del párrafo, si ese es el efecto que deseas. En segundo lugar, puedes especificar dos argumentos para la regla. La primera es la longitud de la línea, y la segunda es el grosor de la línea. Ambas requieren una unidad para ser utilizadas, como "cm" (centímetros) o "pt" (puntos).

### \line

```Latex
\line
```

"\line(x,y){length}" de LaTeX te permite dibujar un segmento de línea en cualquier parte de la página que te gusta, horizontal, o de otra manera. La línea tendrá la longitud definida en el argumento de longitud y pendiente (x, y). Una línea horizontal de 10 centímetros sería "\line(0,0){10 cm}". Sólo puede ser utilizado dentro del entorno "imagen de LaTeX".

### \dotfill

```Latex
\dotfill
```

El comando "\dotfill" permite dibujar una línea de puntos. Esto crea un espacio "rubber" que tendrá un tamaño mínimo de unos pocos puntos, pero se expandirá según sea necesario para llenar el espacio horizontal disponible. Esto es útil para definir una tabla de contenidos donde el título del capítulo está justificado a la izquierda, el número de página justificado a la derecha y el espacio intermedio contiene comando "\dotfill" para llenarlo con puntos. Sin embargo, se puede trazar una línea horizontal de puntos a través de la página si es seguido por el nuevo comando de párrafo "\" .

### \hrulefill

```Latex
\hrulefill
```

El comando "\hrulefill" tiene la misma funcionalidad cono el comando "\dotfill", excepto que llenará el espacio disponible con la "regla horizontal", una línea fina a lo largo de la parte inferior del texto.


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