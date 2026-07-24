------------------------------------------------------------------------

# Ficha de análisis

## 1. Nombre del Space

**Nombre:** MOSS-VL-Realtime

**Enlace:** https://huggingface.co/spaces/OpenMOSS-Team/openmoss-team-moss-vl-realtime

------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

El sistema analiza cada fotograma de un video, y responde cualquier pregunta o da información sobre el material mientras se sigue reproduciendo.

------------------------------------------------------------------------

## 3. Análisis PEAS

  Elemento          Respuesta
  ----------------- ----------------------------------------------------
  **Performance**   se genera una respuesta en tiempo real, con información correcta.
  **Environment**   eventos en el video y lo que se muestra en la toma
  **Actuators**     respuesta, descripción
  **Sensors**       video, imagen

------------------------------------------------------------------------

## 4. Clasificación del entorno

Complete la siguiente tabla y justifique brevemente cada respuesta.

  Propiedad      Clasificación     Justificación
  -------------- ----------------- ---------------
  Observable     Total /  x        Porque el agente solo puede analizar lo que se ve en el video
  Determinista       x / No        Porque el video ya existe, y no cambia por acción del agente
  Episódico         Sí / x         El análisis del video requiere de información en diferentes puntos, por lo que están conectadas
  Estático           X / No        El contenido del video no cambia mientras se analiza
  Discreto          Sí / x         El video es continuo en el tiempo
  Conocido          X  / No        El agente sabe cómo obtener información del video

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Es un agente basado en modelo, porque debe mantener información de todos lo que se muestra en el video, y una representación de la secuencia de eventos para poder dar información en diferentes puntos del video. 
También podría considerarse de objetivo, puesto que su propósito es dar información acertada, en tiempo real, sobre el contenido.


------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**
2.  **Parcialmente observable, estocástico y secuencial.**

Justifique su respuesta.

------------------------------------------------------------------------