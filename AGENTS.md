# Loop :
"""
El proposito de esta sesion es concluir con un paper redactado en latex
sobre los resultados y afirmaciones resultantes de un analisis SHAP sobre
el modelo de clasificacion. El modelo es mobilenetv3_small_050.lamb_in1k y se probo
frente a imagene de un perro Golden Retreiver, un Siberian Husky bebe y una banana
representativos de las imagenes de prueba 1 2 y 3. Asimismo, se realizo un heatmap
para observar los pixeles de mayor influencia. Se puede ver en las imagenes de los perrors
que el modelo asigna mayor peso a las areas como la nariz, las orejas, los ojos. Tambien
es interesante que el contorno tiene absolutamente 0 peso, al punto que el heatmap los mostro 
en 0. Esto sin embargo nos deja observar el mecanismo y as areas de interes de estas categorias.
incluso en la imagen 2 donde confundio la raza del perro por Eskimo y Malamute, estuvo muy cerca
e identifico la naturaleza canina de la imagen. Por ultimo, el heatmap del banano mostro
que las areas de influencia se miran casi aleatorias, no se define el contorno y no hay un enfoque
en areas como las lineas o el tallo, sin embargo, lo clasifico correctamente.

Los resultados fueron:
```
Imagen: images/prueba1.jpg
  golden retriever          86.55%
  Labrador retriever         1.80%
  kuvasz                     1.40%
  Norfolk terrier            1.18%
  Rhodesian ridgeback        0.44%

Imagen: images/prueba2.jpg
  Eskimo dog                31.30%
  malamute                  25.87%
  Siberian husky            12.08%
  Arctic fox                 5.50%
  collie                     2.01%

Imagen: images/prueba3.jpg
  banana                    69.71%
  spaghetti squash           5.40%
  sunglass                   1.05%
  lemon                      1.01%
  whistle                    0.79%
```

El Paper debe estar redactado en latex y tener los siguientes capitulos:
Titulo, Abstract, Introduccion, Metodologia, Resultados, Conclusiones y Referencias.
El estilo debe ser minimalista pero concordante con la estructura de un articulo
en latex: paginas numeradas, 2 columnas de texto, imagenes y tablas correctamente identificadas
y referencias bibliograficas en formato APA.

Aimismo te proveo una lista de las imagenes para que puedas enlazarlas dentro del
archivo tex
```
./images/prueba1.png (golden retreiver)
./images/prueba2.jpg (husky bebe)
./images/prueba3.jpg (banana)
./images/output.png (heatmap SHAP)
```
Trabajaras en un Loop comenzando por una etapa de semilla y continuando
con los pasos siguientes regresando al 1 luego de completar el 4 hasta cumplir
los requisitos de aceptacion.

0. Borrador de contenido y plantilla: realizar la plantilla en latex con
las secciones definidas y con puntos claves relevantes a cada seccion. Esto
servira como semilla para el resto del loop.

1. Verificacion de validez y pertinencia: verificar que el contenido redactado 
sea valido y concordante con las pruebas, que sea valido y pertenezca a su apartado
correspondiente.

2. Coherencia y atribucion: revisar que el paper sea coherente y tenga un flujo
legible de redaccion y que las citas y referencias esten correctamente atribuidas y citadas.

3. Test con latex: probar la renderizacion con latex al archivo main.tex principal
y resolver todos los errores semanticos o programaticos para que compile correctamente y
el estilo concuerde con lo deseado.

4. Redaccion: redaccion de nuevos puntos que consideres relevantes o que sean vacios
en lo discutido y verificacion de que el Abstract sea conistente con las conclusiones.

Los criterios de aceptacion para finalizar la ejecucion del loop son los siguientes
- Redaccion formal y cientifica
- Contenido coherente y relevante
- Titulo breve y explicativo
- Al menos 2 citas formales con APA.
- Inclusion de la tabla de resultados y al menos 2 de las imagenes provistas
- Los capitulos de: Abstract, Introduccion, Metodologia, Resultados, Conclusiones y Referencias.
- Renderizacion en latex sin errores.


 
 