# Aspectos básicos del análisis de texto con el servicio de lenguaje

Para que los sistemas informáticos interpreten el tema de un texto de forma similar, usan el procesamiento del lenguaje natural (NLP), un área dentro de la inteligencia artificial que trata de comprender el idioma escrito o hablado y responder de la misma forma. 

## Descripción de Text Analytics
un cuerpo de texto -> un corpus

### Tokenización
El primer paso para analizar un corpus es dividirlo en tokens. 
En aras de la simplicidad, se puede considerar que cada palabra distinta del texto de entrenamiento es un token

- **Normalización de texto**: Antes de generar tokens, puede optar por normalizar el texto quitando la puntuación y cambiando todas las palabras a minúsculas.
- **Eliminación de palabras vacías**:  Las palabras irrelevantes son palabras que se deben excluir del análisis.
- **n-gramas**: son frases formadas por varios términos, como "yo tengo" o "él camina". 
    - Una frase de una sola palabra es un **unigrama**
    - Una frase de dos palabras es un **bigrama**
    - Una frase de tres palabras es un **trigrama** 
    - etc.
- **lematización**: es una técnica en la que se aplican algoritmos para consolidar palabras antes de contarlas, de modo que las palabras con la misma raíz, como "power", "powered" y "powerful", se interpretan como el mismo token.

### Análisis de frecuencia
Las palabras más usadas a menudo pueden proporcionar una pista sobre el tema principal de un corpus de texto.

El análisis de frecuencia simple en el que simplemente se cuenta el número de repeticiones de cada token puede ser una manera eficaz de analizar un solo documento, pero cuando se necesita diferenciar entre varios documentos dentro del mismo corpus, es necesaria una manera de determinar qué tokens son más relevantes en cada documento

### Aprendizaje automático para la clasificación de textos
Otra técnica de análisis de texto útil es usar un algoritmo de clasificación, como la **regresión logística**, para entrenar un modelo de aprendizaje automático que clasifica el texto basado en un conjunto conocido de categorizaciones. Una aplicación común de esta técnica es entrenar un modelo que **clasifica el texto como positivo o negativo** para realizar **análisis de opiniones o minería de opiniones**.

### Modelos de lenguaje semántico
estos modelos se encuentra la codificación de tokens de lenguaje como vectores (matrices multivalor de números) conocidas como **incrustaciones**.

los elementos de un vector de inserción de tokens son coordenadas en el espacio multidimensional, de modo que cada token ocupa una "ubicación" específica.

En otras palabras, las palabras relacionadas se agrupan más cerca

Entre las tareas comunes de NLP admitidas por los modelos de lenguaje se incluyen las siguientes:

- Análisis de texto, como extraer términos clave o identificar entidades con nombre en texto.
- Análisis de sentimiento y minería de opiniones para clasificar textos como positivo o negativo.
- Traducción automática, en la que el texto se traduce automáticamente de un idioma a otro.
- Resumen, en el que se resumen los puntos principales de un corpus de texto grande.
- Soluciones de inteligencia artificial conversacional, como bots o asistentes digitales en los que el modelo de lenguaje puede interpretar la entrada del lenguaje natural y devolver una respuesta adecuada.

## Introducción al análisis de texto
Lenguaje de Azure AI forma parte de las ofertas de los servicios de Azure AI y puede realizar un procesamiento del lenguaje natural avanzado sobre texto no estructurado.

- **El reconocimiento de entidades** con nombre identifica personas, lugares, eventos y mucho más. Esta característica también se puede personalizar para extraer categorías personalizadas.
- **La vinculación de entidad** identifica entidades conocidas junto con un vínculo a Wikipedia.
- **La detección de información de identificación personal (PII)** identifica información personalmente confidencial, incluida la información personal relacionada con la salud.
- **La detección de idioma** identifica el idioma del texto y devuelve un código de idioma como "en" para inglés.
- **El análisis de sentimiento y la minería de opiniones** identifican si el texto es positivo o negativo.
- **El resumen** resume el texto mediante la identificación de la información más importante.
- **La extracción de frases clave** enumera los conceptos principales del texto no estructurado.