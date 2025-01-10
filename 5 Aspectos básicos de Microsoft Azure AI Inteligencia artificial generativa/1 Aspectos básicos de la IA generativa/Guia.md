# Aspectos básicos de la IA generativa

## ¿Qué es la inteligencia artificial generativa?
La IA generativa describe una categoría de funcionalidades dentro de la inteligencia artificial que crean contenido original. 

Las aplicaciones de IA generativa toman entradas de lenguaje natural y devuelven respuestas adecuadas en diversos formatos, como lenguaje natural, imágenes o código.

- Generación de lenguaje natural
- Generación de imágenes
- Generación de código

## ¿Qué son los modelos de lenguaje?

Las aplicaciones de IA generativa se basan en modelos de lenguaje, que son un tipo especializado de modelo de Machine Learning que se puede usar para realizar tareas de procesamiento de lenguaje natural (NLP), entre las que se incluyen las siguientes:

- Determinar opiniones o clasificar de otro modo un texto de lenguaje natural.
- Resumir un texto.
- Comparar varios orígenes de texto en busca de similitud semántica.
- Generar nuevo lenguaje natural.

### Modelos de transformador

Los modelos de transformador son una arquitectura clave en el procesamiento de lenguaje natural (PLN) y la generación de lenguaje, utilizados en modelos de lenguaje grandes (LLMs) como GPT y BERT. Están diseñados para entender las relaciones semánticas entre palabras y generar texto que tiene sentido. Su funcionamiento se basa en dos bloques principales:

- Bloque codificador: Procesa el texto de entrada (tokens) y crea representaciones vectoriales llamadas incrustaciones, que encapsulan atributos semánticos de los tokens.
- Bloque descodificador: Usa esas incrustaciones para generar secuencias de texto nuevas y coherentes.
### Conceptos principales:
- Tokenización: Divide el texto en unidades básicas (tokens), como palabras o partes de palabras, asignándoles identificadores únicos.
- Incrustaciones: Representaciones vectoriales de los tokens que reflejan relaciones semánticas; palabras similares tienen vectores con orientaciones parecidas.
- Atención: Técnica para analizar relaciones entre tokens. En el codificador, define el contexto semántico de cada token; en el descodificador, predice el siguiente token basado en los anteriores.
### Aplicaciones:
- Modelos como BERT: Usan solo el codificador para tareas como análisis de texto.
- Modelos como GPT: Usan solo el descodificador para generación de lenguaje.

Estas capacidades permiten que los modelos generen texto y realicen tareas complejas al comprender y modelar relaciones entre palabras.

## Uso de modelos de lenguaje

El uso de modelos de lenguaje puede realizarse entrenándolos desde cero o utilizando modelos preexistentes que pueden ajustarse con datos propios. En Microsoft Azure, se ofrecen modelos de lenguaje en el servicio Azure OpenAI y en el catálogo de modelos, que incluyen opciones como GPT-3.5-Turbo, GPT-4, GPT-4 Vision y DALL-E para generación de imágenes. Estos modelos permiten aprovechar una infraestructura segura y escalable.

Los modelos de lenguaje se dividen en dos categorías:

- Modelos de lenguaje grande (LLM):
    - Entrenados con enormes cantidades de datos generales.
    - Poseen miles de millones de parámetros, lo que los hace efectivos en diversos contextos.
    - Su gran tamaño puede complicar implementaciones locales y ajustes personalizados.
- Modelos de lenguaje pequeño (SLM):
    - Entrenados con datos más específicos y de menor escala.
    - Tienen menos parámetros, son más rápidos, más fáciles de ajustar y adecuados para implementaciones locales.
    - Son efectivos en temas específicos, pero menos en contextos generales.

Azure también incluye modelos de código abierto como los de OpenAI, HuggingFace, Meta, y otros.

## ¿Qué son los copilotos?

Los copilotos digitales son asistentes de IA generativa que se integran en aplicaciones como interfaces de chat, ofreciendo soporte contextualizado en tareas comunes. Microsoft Copilot, por ejemplo, se integra en diversas aplicaciones de Microsoft y permite a los desarrolladores crear complementos para personalizar la experiencia o crear copilotos propios.

Los copilotos aumentan la productividad y creatividad al generar contenido y automatizar tareas. Los desarrolladores pueden expandirlos mediante complementos para integrar datos y procesos empresariales o crear copilotos personalizados para aplicaciones específicas.

Existen tres niveles de adopción de copilotos:

- Producto estándar: Uso de copilotos como Microsoft Copilot en aplicaciones como Microsoft 365 para mejorar la productividad.
- Extensión de Microsoft Copilot: Ampliación de funcionalidades para tareas o procesos empresariales personalizados.
- Desarrollo personalizado: Creación de copilotos personalizados para integrar IA generativa en aplicaciones empresariales y ofrecer experiencias únicas a los clientes.

## Microsoft Copilot
Microsoft Copilot integra inteligencia artificial (IA) en diversas aplicaciones de Microsoft para mejorar la productividad y la automatización de tareas. A continuación se destacan algunos de sus usos:

- Exploración web con IA: Copilot en Bing y Edge permite responder preguntas, crear contenido y buscar información relevante, con integración a servicios organizacionales al usar cuentas profesionales.

- Asistencia en aplicaciones de productividad: En Microsoft 365, Copilot ayuda en Word para generar y mejorar documentos, en PowerPoint para crear presentaciones, y en Outlook para resumir correos y organizar tareas.

- Procesos empresariales con IA:
    - Dynamics 365 Customer Service: Moderniza los centros de contacto con IA generativa para mejorar la atención al cliente.
    - Dynamics 365 Sales: Ayuda a los vendedores a gestionar relaciones con clientes mediante análisis rápidos de datos.
    - Dynamics 365 Supply Chain: Optimiza la toma de decisiones sobre compras y cadena de suministro.

- Análisis de datos: En Microsoft Fabric y Power BI, Copilot ayuda a generar códigos y visualizaciones de datos automáticamente.

- Seguridad y administración de TI: Copilot for Security asiste a los profesionales en la evaluación y respuesta a amenazas, y Copilot para Azure ayuda a gestionar la infraestructura en la nube.

- Desarrollo de software: GitHub Copilot ayuda a los desarrolladores generando, explicando y documentando código, y también sugiriendo mejoras.

Copilot busca mejorar la productividad y creatividad de los usuarios al integrar IA en diversas aplicaciones empresariales y personales.