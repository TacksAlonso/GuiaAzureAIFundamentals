# Aspectos básicos del reconocimiento óptico de caracteres
## Comenzar con Visión de Azure AI 
El reconocimiento óptico de caracteres (OCR) es la base del procesamiento de texto en imágenes y usa modelos de Machine Learning entrenados para reconocer formas individuales como letras, números, puntuación u otros elementos de texto. 

### Motor de OCR de Visión de Azure AI
El servicio Visión de Azure AI tiene la capacidad de extraer texto legible por máquina de imágenes. Read API de Visión de Azure AI es el motor de OCR que permite extraer texto de imágenes, archivos PDF y TIFF. El OCR para imágenes está optimizado para imágenes generales, no de documentos, que facilitan la inserción de OCR en escenarios de experiencia de usuario.

Read API, también conocida como motor Read OCR, usa los últimos modelos de reconocimiento y está optimizada para imágenes que tienen una cantidad significativa de texto o un ruido visual considerable. 

Al llamar a Read API, se devuelven los resultados organizados en la siguiente jerarquía:

- Páginas: un resultado por cada página de texto, con información sobre el tamaño y la orientación de la página.
- Líneas: las líneas de texto de una página.
- Palabras: palabras de una línea de texto, incluidas las coordenadas del cuadro de límite y el propio texto.

## Introducción a Vision Studio en Azure
formas de usar Read API de Visión de Azure AI:

- Vision Studio
- REST API
- Kits de desarrollo de software (SDK): Python, C#, JavaScript