# Aspectos básicos de Minería de conocimiento y Búsqueda de Azure AI
## ¿Qué es Azure AI Search?
proporciona la infraestructura y las herramientas necesarias para crear soluciones de búsqueda que permitan extraer datos de una variedad de documentos estructurados, semiestructurados y no estructurados.

Los resultados de Búsqueda de Azure AI contienen solo los datos, que pueden incluir el texto deducido o extraído de imágenes, o nuevas entidades y detección de frases clave mediante el análisis de texto. Se trata de una solución de plataforma como servicio (PaaS). 

### Características de Búsqueda de Azure AI
- **Datos de cualquier origen**: acepta datos de cualquier origen proporcionados en formato JSON, con soporte de rastreo automático de orígenes de datos seleccionados en Azure.
- **Varias opciones para la búsqueda y el análisis**: incluida la búsqueda vectorial, el texto completo y la búsqueda híbrida.
- **Enriquecimiento con IA**: tiene funcionalidades de Azure AI integradas para el análisis de imágenes y texto a partir de contenido sin procesar.
- **Análisis lingüístico**: ofrece un análisis lingüístico de 56 idiomas que controla de manera inteligente la lingüística específica del idioma o la coincidencia fonética. Los procesadores de lenguaje natural disponibles en Búsqueda de Azure AI también los usan Bing y Office.
- **Experiencia de usuario configurable**: dispone de opciones para la sintaxis de las consultas, como consultas vectoriales, búsqueda de texto, consultas híbridas, búsqueda aproximada, autocompletado, filtrado de búsqueda geográfica en función de la proximidad a una ubicación física, etc.
- **Escala, seguridad e integración de Azure**: en la capa de datos, la capa de aprendizaje automático y con los servicios de Azure AI y Azure OpenAI.

## Identificación de elementos de una solución de búsqueda
Un índice de búsqueda en Azure AI Search almacena contenido que se puede buscar. Para crearlo, se utiliza una canalización de indexación que incluye los siguientes pasos:

- Origen de datos: Es la ubicación de los datos originales (como Azure Storage, Azure SQL Database o Azure Cosmos DB) que contiene archivos PDF, imágenes, videos, o texto.

- Indexador: Automatiza el proceso de extracción y transformación de datos del origen, descifra documentos, y los convierte a JSON (serialización de JSON).

- Descifrado de documentos: Extrae el contenido de los archivos originales.

- Enriquecimiento con IA: Aplica capacidades de inteligencia artificial (como OCR, traducción de texto o análisis de sentimientos) para extraer información adicional. El contenido enriquecido puede almacenarse en un almacén de conocimiento para análisis adicional.

- Inserción en el índice: Los datos procesados en formato JSON se usan para rellenar el índice de búsqueda.

El índice de búsqueda resultante tiene una estructura similar a una tabla con un esquema que define campos, tipos de datos y atributos (como filtrado o clasificación). Esto permite a los usuarios buscar información (por ejemplo, "coffee") de manera eficiente en el índice.

## Uso del Asistente para importación de datos de Azure Portal

El Asistente para importación de datos en Azure Portal simplifica la creación de los objetos necesarios para el motor de búsqueda en el servicio Azure AI Search. Este asistente automatiza los procesos de definición del índice de búsqueda y ejecución del indexador. Los principales objetos que gestiona son:

- Origen de datos: Almacena la conexión a los datos originales (incluidas credenciales) y se utiliza exclusivamente con indexadores.

- Índice: Es la estructura física donde se realizan búsquedas de texto completo y otras consultas.

- Indexador: Configura la conexión entre el origen de datos y el índice de destino, especificando también un conjunto opcional de aptitudes de IA, programación, y valores para la gestión de errores o codificación.

- Conjunto de aptitudes: Define las operaciones de manipulación y enriquecimiento de contenido (como extracción de texto de imágenes o análisis de datos) mediante recursos de Azure AI.

- Almacén de conocimiento: Almacena los datos enriquecidos con IA en tablas o blobs de Azure Storage para análisis adicional o procesamiento.

Este asistente es especialmente útil para automatizar y gestionar los flujos de trabajo de indexación y enriquecimiento de datos en Azure AI Search.