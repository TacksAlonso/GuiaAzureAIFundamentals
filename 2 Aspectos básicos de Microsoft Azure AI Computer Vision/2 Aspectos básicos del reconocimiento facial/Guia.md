# Aspectos básicos del reconocimiento facial

## Descripción del análisis facial
La detección de caras implica la identificación de regiones de una imagen que contienen un rostro humano, generalmente al devolviendo las coordenadas de cuadro de límite que forman un rectángulo alrededor de la cara

### Reconocimiento facial
con el análisis facial se puede entrenar un modelo Machine Learning para identificar individuos conocidos a partir de sus rasgos faciales

### Introducción al análisis facial en Azure
Microsoft Azure proporciona varios servicios de Azure AI que puede usar para detectar y analizar caras, entre los que se incluyen:
- Visión de Azure AI, que ofrece detección de caras y algunos análisis básicos de caras, como devolver las coordenadas del rectángulo delimitador alrededor de una imagen.
- Video Indexer de Azure AI, que puede usar para detectar e identificar caras en un vídeo.
- Face de Azure AI, que ofrece algoritmos pregenerados que pueden detectar, reconocer y analizar caras.

### Servicio Face de Azure AI
El servicio Face de Azure AI puede devolver coordenadas de rectángulo para cualquier cara humana que se encuentre en una imagen

- Accesorios: indica si la cara dada tiene accesorios. Este atributo devuelve posibles accesorios, incluidos artículos para la cabeza, gafas y mascarilla, con una puntuación de confianza entre cero y uno para cada accesorio.
- Desenfoque: qué grado de desenfoque tiene la cara, que puede ser una indicación de la probabilidad de que la cara sea el foco principal de la imagen.
- Exposición: por ejemplo, si la imagen está infraexpuesta o sobreexpuesta. Esto se aplica a la cara de la imagen y no a la exposición general de la imagen.
- Gafas: si la persona lleva gafas o no.
- Posición de la cabeza: la orientación de la cara en un espacio 3D.
- Máscara: indica si la cara está usando una máscara.
- Ruido: hace referencia al ruido visual de la imagen. Si ha tomado una foto con una configuración ISO alta para entornos más oscuros, notará este ruido en la imagen. La imagen se ve granulada o repleta de pequeños puntos que hacen que la imagen sea menos clara.
- Oclusión: determina si puede haber objetos que bloqueen la cara en la imagen.
- Calidad del reconocimiento: una clasificación de alta, media o baja que refleja si la imagen tiene la calidad suficiente para intentar el reconocimiento facial.

La directiva de acceso limitado requiere que los clientes envíen un formulario de entrada para acceder a funcionalidades adicionales del servicio Face de Azure AI, como:

- Verificación facial: la capacidad de comparar caras en busca de similitudes.
- Identificación facial: la capacidad de identificar individuos con nombre en una imagen.
- Detección de vida: capacidad de detectar y mitigar casos de contenidos y/o comportamientos recurrentes que indiquen una violación de las directivas (por ejemplo, si el flujo de vídeo de entrada es real o falso).