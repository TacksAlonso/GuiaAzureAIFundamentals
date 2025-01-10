# Aspectos básicos de Documento de inteligencia de Azure AI
La inteligencia de documentos describe las funcionalidades de inteligencia artificial que admiten el procesamiento de texto y que dan sentido a la información contenida en ellos. Como extensión del reconocimiento óptico de caracteres (OCR), la inteligencia de documentos da el siguiente paso que una persona podría dar después de leer un formulario o documento. Automatiza el proceso de extracción, comprensión y guardado de los datos en texto.

## Exploración de funcionalidades de inteligencia de documentos
La inteligencia de documentos se basa en modelos de aprendizaje automático entrenados para reconocer datos en texto. La capacidad de extraer pares de texto, diseño y clave-valor se conoce como **análisis de documentos**. El análisis de documentos proporciona ubicaciones de texto en una página identificada mediante coordenadas de cuadro de límite.

## Descripción de funcionalidades de Documento de inteligencia de Azure AI

El documento de inteligencia de Azure AI consta de características agrupadas por tipo de modelo:

- Análisis de documentos: análisis general de documentos que devuelve representaciones de datos estructuradas, incluidas las regiones de interés y sus interrelaciones.
- Modelos precompilados: modelos previamente entrenados que se han compilado para procesar tipos de documentos comunes como facturas, tarjetas de presentación, documentos de identidad, etc. Estos modelos están diseñados para reconocer y extraer campos específicos que son importantes para cada tipo de documento.
- Modelos personalizados: se pueden entrenar para identificar campos específicos que no se incluyen en los modelos previamente entrenados existentes. Incluye modelos de clasificación personalizados y modelos de extracción de campos de documento, como el modelo de IA generativa personalizado y el modelo neuronal personalizado.

### Modelos creados previamente

Los modelos precompilados aplican aprendizaje automático avanzado para identificar y extraer con precisión texto, pares clave-valor, tablas y estructuras de formularios y documentos