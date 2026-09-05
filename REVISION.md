# Registro de revisión

## Semilla

Se preparó `main.tex` como artículo de dos columnas, con título breve, Abstract, Introducción, Metodología, Resultados, Conclusiones y Referencias. Se incorporaron la tabla de quince predicciones, las tres entradas y el heatmap original.

## Primera iteración

1. **Validez y pertinencia.** Se contrastaron los quince porcentajes con las salidas de `main.ipynb` y se inspeccionaron las cuatro imágenes. El cuaderno documenta CPU, preprocesamiento, referencia de tres imágenes, 50 muestras y explicación del logit ganador. No se ejecutó nuevamente la inferencia.
2. **Coherencia y atribución.** Se consultaron las publicaciones de Lundberg y Lee (2017) y Howard et al. (2019), la documentación oficial de GradientExplainer y la ficha del modelo en timm. Se incorporaron cuatro referencias en formato autor-fecha APA, ordenadas alfabéticamente, con enlaces.
3. **LaTeX.** La compilación inicial detectó una orden matemática no definida; se corrigió. Se resolvieron referencias cruzadas y un desbordamiento de URL. MiKTeX requirió permiso para escribir sus registros y cachés en el perfil del usuario.
4. **Redacción.** Se explicitaron las diferencias entre logits y softmax, el significado de los signos, las escalas independientes, la posible cancelación de canales y la superposición sin invertir el recorte. Se revisó que el Abstract reflejara las conclusiones.

## Segunda iteración

1. Se comprobaron los márgenes entre clases (84,75; 5,43; 64,31 puntos porcentuales) y la suma de las primeras tres clases del cachorro (69,25 %). Se evitó presentar estos tres casos como una evaluación generalizable.
2. Se revisaron las atribuciones bibliográficas y la correspondencia entre las afirmaciones y las fuentes. La ausencia de color no se presenta como prueba de cero exacto; el patrón disperso de la banana no se considera aleatoriedad demostrada. El mapa del cachorro explica Eskimo dog, no un contraste entre razas.
3. Se recompiló el documento y se inspeccionaron las páginas renderizadas para comprobar columnas, numeración, figuras, tabla y referencias.
4. Se retiró del cuerpo del artículo una aclaración editorial sobre extensiones de archivo, conservándola en README. La revisión final mantuvo la coherencia entre objetivo, resultados, limitaciones y conclusiones.

## Criterios de aceptación

- Redacción formal y científica, con alcance exploratorio explícito.
- Título breve y explicativo.
- Todas las secciones solicitadas.
- Cuatro fuentes citadas en el texto y referenciadas en APA.
- Tabla con las cinco clases de cada una de las tres imágenes.
- Inclusión de las tres imágenes y el heatmap, en dos figuras numeradas y citadas.
- Artículo en dos columnas y páginas numeradas.
- PDF compilado con pdfLaTeX; revisar `main.log` para el registro técnico de la última compilación.

La ausencia de versiones, semillas y arreglos de atribución guardados limita la reproducción numérica del experimento, pero no la compilación del artículo.
