# Aspectos básicos de Voz de Azure AI
Las funcionalidades de voz de IA nos permiten administrar sistemas domésticos y automáticos con instrucciones de voz, obtener respuestas de ordenadores para preguntas orales, generar subtítulos a partir de audio y mucho más.

## Descripción del reconocimiento y la síntesis de voz
### Descripción del reconocimiento
El reconocimiento de voz toma la palabra hablada y la convierte en datos que se pueden procesar, a menudo transcribiéndolos en texto. 

El texto oral puede tener el formato de voz grabada en un archivo de audio o de audio en directo procedente de un micrófono. Los patrones de voz se analizan en el audio para determinar patrones reconocibles que se asignan a palabras. Para conseguirlo, el software suele usar varios modelos, entre los que se incluyen:

- **Un modelo acústico** que convierte la señal de audio en fonemas (representaciones de sonidos específicos).
- **Un modelo lingüístico** que asigna fonemas a palabras, normalmente mediante un algoritmo estadístico que predice la secuencia más probable de palabras en función de los fonemas.

### La síntesis de voz
Hace referencia a los datos de vocalizaciones, normalmente convirtiendo texto a voz

Para sintetizar la voz, el sistema suele acortar el texto para dividirlo en palabras individuales y asigna sonidos fonéticos a cada palabra.

## Introducción a la voz en Azure
Microsoft Azure ofrece funcionalidades de reconocimiento de voz y síntesis a través de servicio Azure AI Speech, que admite muchas funcionalidades, entre las que se incluyen:

- Speech to Text
- Text to speech

### Speech to Text
Puede usar la API de conversión de voz en texto de Azure AI para realizar transcripciones de audio en tiempo real o por lotes a un formato de texto. 

La fuente de audio de la transcripción puede ser una transmisión de audio en tiempo real desde un micrófono o un archivo de audio.

- **Transcripción en tiempo real**: La conversión de voz en texto en tiempo real le permite transcribir el texto en secuencias de audio. Puede usar la transcripción en tiempo real para presentaciones, demostraciones o cualquier otra situación en la que una persona hable.

- **Transcripción de Batch**: No todos los escenarios de conversión de voz en texto son en tiempo real. Es posible que tenga grabaciones de audio almacenadas en un recurso compartido de archivos, en un servidor remoto o incluso en almacenamiento de Azure. Puede apuntar a archivos de audio con un URI de firma de acceso compartido (SAS) y recibir resultados de transcripción de forma asincrónica.

### Text to speech

La API Text to Speech le permite convertir la entrada de texto en voz audible, que puede reproducirse directamente a través del altavoz de un equipo o escribirse en un archivo de audio.

**Voces de síntesis de voz**: Cuando usa la API Text to Speech, puede especificar la voz que se usará para vocalizar el texto. Esta opción le ofrece la flexibilidad de personalizar la solución de síntesis de voz y darle un carácter concreto.