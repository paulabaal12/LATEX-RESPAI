# Atribuciones SHAP en MobileNetV3

Artículo en español sobre las predicciones y explicaciones de tres imágenes con `mobilenetv3_small_050.lamb_in1k`.

- Fuente editable: [main.tex](main.tex).
- Artículo compilado: [main.pdf](main.pdf).
- Evidencia del procedimiento y resultados: [main.ipynb](main.ipynb).
- Revisión del artículo: [REVISION.md](REVISION.md).

## Compilación

Desde la carpeta del proyecto, ejecutar dos veces para resolver las referencias cruzadas:

```powershell
pdflatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

Se requiere una distribución LaTeX con los paquetes `babel` (español), `geometry`, `graphicx`, `amsmath`, `url` e `hyperref`. Las referencias APA están incluidas en `main.tex`; no se requiere BibTeX ni Biber. Conservar la carpeta `images` junto al documento. La imagen del golden retriever disponible es `images/prueba1.jpg`.

El artículo utiliza las salidas guardadas del experimento; su compilación no vuelve a ejecutar el modelo ni SHAP. Las observaciones visuales se distinguen de las hipótesis y se documentan las limitaciones del procedimiento.
