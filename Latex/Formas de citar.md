														16-08-2023

>[!cite] Índice: [[Índice LaTex]]

# Formas de citar

En LaTeX, hay varias formas de citar referencias bibliográficas en tu documento, y la elección depende del estilo de citación que desees utilizar y de cómo quieras que aparezcan las citas en el texto. Aquí hay algunas formas comunes de citar en LaTeX:

1. **Citar en el texto con el nombre del autor:**
   - Uso: `\textcite{referencia}`
   - Ejemplo: `\textcite{Smith2020}` generará "Smith (2020) encontró que..."

2. **Citar en el texto con el número de referencia:**
   - Uso: `\cite{referencia}`
   - Ejemplo: `\cite{Jones2018}` generará "[1]".

3. **Citar entre paréntesis con el nombre del autor y el año:**
   - Uso: `\parencite{referencia}`
   - Ejemplo: `\parencite{Brown2015}` generará "(Brown, 2015)".

4. **Citar entre paréntesis solo con el número de referencia:**
   - Uso: `\parencite{referencia}`
   - Ejemplo: `\parencite{Garcia2019}` generará "(2)".

5. **Citar de manera indirecta:**
   - Uso: `\citetitle{referencia}`
   - Ejemplo: `\citetitle{Johnson2008}` generará "El título del artículo de Johnson (2008) es..."

6. **Citar solo el nombre del autor en el texto:**
   - Uso: `\citeauthor{referencia}`
   - Ejemplo: `\citeauthor{Taylor2017}` generará "Taylor".

7. **Citar solo el año en el texto:**
   - Uso: `\citeyear{referencia}`
   - Ejemplo: `\citeyear{Miller2016}` generará "2016".

8. **Citar con número de página específico:**
   - Uso: `\cite[página]{referencia}`
   - Ejemplo: `\cite[p. 28]{Williams2022}` generará "[3, p. 28]".

9. **Citar varias referencias en una sola cita:**
   - Uso: `\cite{referencia1, referencia2, ...}`
   - Ejemplo: `\cite{Smith2020, Jones2018}` generará "[1, 2]".

10. **Citar sin paréntesis:**
   - Uso: `\nocite{referencia}`
   - Ejemplo: `\nocite{Adams2014}` agrega la referencia a la lista de referencias sin citarla en el texto.

Estos son solo algunos ejemplos de cómo puedes citar en LaTeX. La forma en que cites dependerá de las normas de estilo que estés siguiendo y de tus preferencias personales. Asegúrate de consultar la documentación del paquete `biblatex` y los requisitos de citación de tu institución o revista para asegurarte de que estás aplicando la citación de manera correcta y coherente en tu documento.


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


--------------------------------------------------

# Etiquetas
> [!info] Etiquetas
> - #LaTex 
> - Etiqueta 2