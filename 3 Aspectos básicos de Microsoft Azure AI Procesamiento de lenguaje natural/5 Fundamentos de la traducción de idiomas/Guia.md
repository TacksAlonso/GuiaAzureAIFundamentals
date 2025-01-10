# Fundamentos de la traducción de idiomas
## Comprender conceptos de traducción
Uno de los muchos retos de la traducción es que las palabras no tienen una correspondencia exacta entre idiomas.

### Traducción literal y semántica
Los primeros intentos de traducción automática fueron traducciones literales. En una traducción literal, cada palabra se traduce por la palabra correspondiente en el idioma de destino.

Los sistemas de inteligencia artificial deben ser capaces de comprender, no solo las palabras, sino también el contexto semántico en el que se utilizan.

### Traducción de texto y voz

La **traducción de texto** se puede usar para traducir documentos de un idioma a otro, comunicaciones de correo electrónico que provienen de gobiernos extranjeros e, incluso, páginas web en Internet.

La **traducción de voz** se utiliza para traducir la voz, a veces directamente (traducción de voz a voz) y otras a un formato de texto intermedio (traducción de voz a texto).

## Descripción de la traducción en Azure

Microsoft proporciona servicios de Azure AI que admiten la traducción. Concretamente, puede usar los siguientes servicios:

- El servicio Traductor de Azure AI, con el que podrá traducir un texto a otro texto.
- El servicio Voz de Azure AI, con el que podrá convertir los mensajes de voz en texto o traducir la voz.

### Traductor de Azure AI
Traductor de Azure AI es fácil de integrar en sus aplicaciones, sitios web, herramientas y soluciones. Este servicio usa un modelo de traducción automática neuronal (NMT) para la traducción, que analiza el contexto semántico del texto para ofrecer, como resultado, una traducción más precisa y completa.

### Voz de Azure AI
Puede usar Voz de Azure AI para traducir audio de voz desde una fuente de streaming, como un micrófono o un archivo de audio, y obtener la traducción como texto o en una transmisión de audio. Esto permite escenarios como los subtítulos (CC) en tiempo real para un discurso o la traducción simultánea bidireccional de una conversación hablada.

## Introducción a la traducción en Azure
### Uso del Traductor de Azure AI
Traductor de Azure AI incluye las siguientes funcionalidades:

- **Traducción de texto**: se usa para la traducción rápida y precisa de texto en tiempo real en todos los idiomas admitidos.
- **Traducción de documentos**: se usa para traducir varios documentos en todos los idiomas admitidos, a la vez que se conserva la estructura original del documento.
- **Traducción personalizada**: se usa para permitir que empresas, desarrolladores de aplicaciones y proveedores de servicios de lenguaje creen sistemas de traducción automática neuronal (NMT) personalizados.

La interfaz de programación de aplicaciones (API) de Traductor de Azure AI ofrece una configuración opcional que le ayuda a ajustar los resultados que se devuelven, entre los que se incluyen:

- **Filtrado de lenguaje obsceno**. Sin ninguna configuración, el servicio traducirá el texto de entrada sin filtrar el lenguaje obsceno. Los niveles de lenguaje obsceno suelen ser específicos de cada cultura, pero puede controlar su traducción marcando el texto traducido como obsceno u omitiéndolo en los resultados.
- **Traducción selectiva**. Puede etiquetar contenido para que no se traduzca. Por ejemplo, es posible que quiera etiquetar un código, un nombre de marca o una palabra o frase que no tiene sentido al traducir.

### Traducción de voz con Voz de Azure AI

- La conversión de voz en texto se usa para transcribir la voz de una fuente de audio a formato de texto.
- La conversión de texto a voz se usa para generar audio de voz a partir de una fuente de texto.
- La traducción de voz se utiliza para traducir mensajes de voz de un idioma a mensajes de texto o voz en otro.