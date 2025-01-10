# Computer Vision

## Imágenes y procesamiento de imágenes
### Qué es una imagen en el contexto informático
- Una imagen se representa como una matriz de valores numéricos (píxeles).
- En imágenes en escala de grises, los valores de píxeles van de 0 (negro) a 255 (blanco).
- Una imagen de color incluye tres capas (canales) para representar tonos de rojo, verde y azul (RGB). 
### Uso de filtros en el procesamiento de imágenes
Los filtros modifican valores de píxeles para aplicar efectos visuales.
Se definen mediante matrices (kernels). Ejemplo de un kernel 3x3:
```diff
-1 -1 -1
-1  8 -1
-1 -1 -1
```

El kernel se aplica a la imagen original mediante convolución, calculando sumas ponderadas para crear una nueva matriz de píxeles.
El filtrado convolucional puede:
Resaltar bordes (como con el filtro Laplace).
Crear desenfoques, nitidez, invertir colores, entre otros efectos.
### Ejemplo de filtro aplicado
Una matriz de escala de grises es procesada con un kernel que resalta los bordes.
El resultado es una nueva imagen con los bordes destacados.
Este tipo de procesamiento es clave en visión por ordenador para analizar y transformar imágenes.

## Aprendizaje automático para Computer Vision
La capacidad de usar filtros para aplicar efectos a imágenes resulta útil en tareas de procesamiento de imágenes, como podría realizar con software de edición de imágenes.

### Redes neuronales convolucionales (CNN)
Las CNN usan filtros para extraer mapas numéricos de características de imágenes y, a continuación, introducen los valores de características a un modelo de aprendizaje profundo para generar una predicción de etiquetas.

### Transformadores y modelos multimodales
Las CNN han estado en el núcleo de las soluciones de Computer Vision durante muchos años. Aunque normalmente se usan para resolver problemas de clasificación de imágenes como se ha descrito anteriormente, también son la base de modelos de Computer Vision más complejos. 

### Transformadores
Los transformadores funcionan mediante el procesamiento de grandes volúmenes de datos y tokens de lenguaje de codificación (que representan palabras o frases individuales) como incrustaciones basadas en vectores (matrices de valores numéricos). 

una **inserción** como una representación de un conjunto de dimensiones donde cada una representa algún atributo semántico del token.

Los tokens que son semánticamente similares se codifican en posiciones similares, creando un modelo de lenguaje semántico que permite crear soluciones sofisticadas de NLP para el análisis de texto, la traducción, la generación de lenguajes y otras tareas.

### Modelos multimodales
el modelo se entrena mediante un gran volumen de imágenes con descripción, sin etiquetas fijas. Un codificador de imágenes extrae características de imágenes basadas en valores de píxeles y las combina con incrustaciones de texto creadas por un codificador de lenguaje. El modelo general encapsula las relaciones entre las incrustaciones de tokens de lenguaje natural y las características de imagen

El modelo de Microsoft Florence es simplemente un modelo de este tipo.

se puede usar Florence como modelo de base para los modelos adaptables que realizan:

- **Clasificación de imágenes**: Identificación de la categoría a la que pertenece una imagen.
- **Detección de objetos**: Buscar objetos individuales dentro de una imagen.
- **Subtitulado**: Generar descripciones adecuadas de imágenes.
- **Etiquetado**: Compilar una lista de etiquetas de texto relevantes para una imagen.

## Visión de Azure AI
El servicio Visión de Azure AI de Microsoft proporciona modelos de Computer Vision precompilados y personalizables basados en el modelo de base Florence y proporcionan diversas funcionalidades eficaces

### Recursos de Azure para el servicio Visión de Azure AI
debe crear un recurso para él en la suscripción de Azure
- Visión de Azure AI
- Servicios de Azure AI

### Analizar imágenes con el servicio Visión de Azure AI
Visión de Azure AI admite varias funcionalidades de análisis de imágenes, entre las que se incluyen:

- Reconocimiento óptico de caracteres (OCR): extrayendo texto de imágenes.
- Generar subtítulos y descripciones de imágenes.
- Detección de miles de objetos comunes en imágenes.
- Etiquetado de características visuales en imágenes