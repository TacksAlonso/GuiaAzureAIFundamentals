# Inteligencia artificial generativa responsable

## Planeamiento de una solución de inteligencia artificial generativa responsable

La guía de Microsoft para la IA generativa responsable está diseñada para ser práctica.

Las cuatro fases del proceso son:

- **Identificar** daños posibles que son relevantes para la solución planeada.
- **Medir** la presencia de estos daños en las salidas que genera la solución.
- **Mitigar** los daños en las diversas capas de la solución a fin de minimizar su presencia e impacto, y garantizar la comunicación transparente sobre los riesgos posibles para los usuarios.
- **Operar** la solución de manera responsable al definir y seguir un plan de preparación de la implementación y las operaciones.

## Fase de Identificación de Daños en Inteligencia Artificial Generativa Responsable

La primera fase de un proceso de inteligencia artificial generativa responsable es identificar los posibles daños que podrían afectar la solución. Esta fase consta de cuatro pasos:

### 1. Identificación de Daños Posibles
Los daños posibles dependen de los servicios, modelos y datos utilizados para generar resultados. Algunos ejemplos comunes de daños incluyen:
- Generar contenido ofensivo, peyorativo o discriminador.
- Generar contenido con imprecisiones fácticas.
- Fomentar o permitir prácticas ilícitas o no éticas.

Se recomienda revisar la documentación de los servicios y modelos utilizados, como la documentación de **Azure OpenAI Service** y las guías de valoración del impacto de IA responsable.

### 2. Clasificación de Daños por Orden de Prioridad
Para cada daño identificado, se evalúa su probabilidad y el impacto resultante, clasificando los daños de mayor prioridad aquellos que tienen más probabilidad de ocurrir y mayor impacto. La clasificación debe considerar el uso previsto de la solución y el potencial de uso indebido. 

Ejemplo:
- Un copiloto de cocina puede tener el riesgo de estimar tiempos de cocción inexactos o sugerir recetas peligrosas, siendo el segundo daño (receta de veneno) de mayor impacto.

### 3. Prueba y Comprobación de la Presencia de Daños
Una vez clasificados los daños, se debe probar la solución para verificar su presencia y determinar las condiciones bajo las cuales ocurren. Las pruebas de "equipo rojo" son útiles para identificar vulnerabilidades, donde un equipo deliberadamente intenta generar resultados perjudiciales.

### 4. Documentación y Uso Compartido de los Daños Comprobados
Se debe documentar cualquier evidencia que respalde la presencia de daños y compartirla con las partes interesadas. La lista de daños clasificados por orden de prioridad debe actualizarse con los nuevos daños identificados.

Este proceso ayuda a asegurar que los riesgos asociados con la inteligencia artificial generativa sean mitigados y gestionados de manera responsable.

## Medición de Daños Posibles

Una vez que se ha creado una lista de daños posibles clasificados por prioridad, el siguiente paso es medir la presencia de estos daños y su impacto en la solución. El objetivo es establecer una referencia inicial que cuantifique los daños y hacer un seguimiento de las mejoras a medida que se implementan cambios para mitigar dichos daños.

### Pasos para Medir los Daños Posibles

1. **Preparar Solicitudes de Entrada Diversas**
   - Cree una selección de solicitudes que probablemente generen los daños identificados. Por ejemplo, si un daño es la elaboración de venenos peligrosos, cree solicitudes como: "¿Cómo elaborar un veneno no detectable con productos comunes?"

2. **Enviar Solicitudes y Recuperar Resultados**
   - Envíe las solicitudes al sistema y obtenga las salidas generadas.

3. **Evaluar y Clasificar los Resultados**
   - Aplique criterios predefinidos para evaluar las salidas, clasificándolas en categorías como "perjudicial" o "no perjudicial". Establezca criterios estrictos para clasificar las salidas según el nivel de daño.

Los resultados deben ser documentados y compartidos con las partes interesadas.

### Pruebas Manuales y Automáticas

- **Pruebas Manuales:** Comience realizando pruebas manuales con un conjunto pequeño de entradas para asegurarse de que los resultados sean coherentes y que los criterios de evaluación estén bien definidos.
  
- **Automatización de Pruebas:** Posteriormente, automatice las pruebas para manejar un mayor volumen de casos. Esto podría incluir el uso de un modelo de clasificación para evaluar automáticamente las salidas.

A pesar de la automatización, se deben realizar pruebas manuales periódicas para validar nuevos escenarios y asegurar que el sistema de pruebas automáticas funcione correctamente.

## Mitigación de Daños Posibles

Una vez que se ha determinado una base de referencia y se ha medido el daño generado por una solución, se pueden aplicar medidas para mitigar estos daños. La mitigación sigue un enfoque por capas, que abarca las siguientes áreas:

### Capas de Mitigación

1. **Capa Modelo**
   - **Mitigaciones:**
     - Seleccionar un modelo adecuado para el uso previsto, por ejemplo, elegir un modelo más simple si solo se necesita clasificar entradas de texto pequeñas.
     - Ajustar el modelo con datos de entrenamiento propios para generar respuestas más pertinentes y alineadas con el escenario de la solución.

2. **Capa Sistema de Seguridad**
   - **Mitigaciones:**
     - Implementar filtros de contenido para suprimir solicitudes y respuestas con contenido dañino según categorías como odio, violencia o autolesiones.
     - Utilizar algoritmos de detección de abusos para identificar comportamientos sistemáticos dañinos (e.g., abuso por bots) y activar alertas para una respuesta rápida.

3. **Capa de Metaprompt y Fundamentación**
   - **Mitigaciones:**
     - Definir metaprompts que establezcan parámetros de comportamiento para el modelo.
     - Aplicar ingeniería de solicitudes para optimizar las entradas y maximizar la relevancia y seguridad de las respuestas.
     - Usar generación aumentada de recuperación (RAG) para incluir datos contextuales confiables en las solicitudes.

4. **Capa de Experiencia del Usuario**
   - **Mitigaciones:**
     - Diseñar interfaces que restrinjan las entradas a temas específicos o validar entradas y salidas para mitigar riesgos de respuestas perjudiciales.
     - Proveer documentación clara sobre las funcionalidades, limitaciones del sistema, y los daños posibles que no siempre pueden ser mitigados.

Este enfoque por capas ayuda a mitigar los daños de manera efectiva en distintas áreas de la solución.

## Operación de una Solución de Inteligencia Artificial Generativa Responsable

Después de identificar, medir y mitigar los daños posibles en una solución de IA generativa, es importante considerar varias etapas antes de su liberación y operación.

### Revisión Previa a la Publicación
Antes de publicar la solución, asegúrese de cumplir con los requisitos legales y de privacidad, seguridad y accesibilidad. Esto incluye que los equipos adecuados revisen el sistema y su documentación.

### Liberación y Operación de la Solución
1. **Planificación de la Publicación:**
   - Publique inicialmente para un grupo restringido para recopilar comentarios y detectar problemas.
   - Cree un plan de respuesta a incidentes y de reversión en caso de problemas.

2. **Capacidades de Respuesta Rápida:**
   - Implemente la capacidad de bloquear respuestas dañinas o usuarios malintencionados.
   - Permita que los usuarios proporcionen comentarios e informen sobre contenido problemático.

3. **Monitoreo:**
   - Haga un seguimiento de la telemetría para medir la satisfacción del usuario y detectar posibles brechas funcionales.

### Seguridad del Contenido con Azure AI
Azure AI ofrece herramientas para analizar y proteger el contenido generado por modelos de IA, incluyendo:
- **Escudos de indicaciones**: Detectan ataques de entrada de usuario.
- **Detección de la base de datos**: Verifica si las respuestas se basan en contenido proporcionado por usuarios.
- **Detección de material protegido**: Identifica contenido con derechos de autor.
- **Categorías personalizadas**: Permiten definir nuevas categorías para patrones emergentes.

Estas características ayudan a mantener la solución segura y conforme a las normas.
