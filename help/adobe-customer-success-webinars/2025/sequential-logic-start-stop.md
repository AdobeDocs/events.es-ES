---
title: 'Dominio de la lógica secuencial en Adobe Analytics y Customer Journey Analytics: inicios y paradas'
description: Domine la lógica secuencial en Adobe Analytics con segmentación avanzada, controles de ámbito y campos derivados para descubrir patrones de comportamiento de los clientes y mejorar la precisión de los datos.
solution: Analytics, Customer Journey Analytics
role: Developer
level: Intermediate
doc-type: Event
duration: 3370
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18017
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Dominio de la lógica secuencial en Adobe Analytics y Customer Journey Analytics: Inicios y detenciones

En esta sesión, exploraremos cómo configurar secuencias con el operador THEN en Adobe Analytics (AA) y Customer Journey Analytics (CJA). Aprenda a recuperar subconjuntos precisos de actividad combinando SOLO DESPUÉS/SOLO ANTES DE LA SECUENCIA con los puntos de comprobación EXCLUIR.

## Puntos de debate

* Revisión rápida de los operadores de lógica secuencial independientes y del marco visual.
* Describa cómo EXCLUIR afecta a los resultados de las secuencias utilizando SOLO DESPUÉS/ANTES DE LA SECUENCIA.
* Presente casos de uso y demostraciones que muestren cómo puede adoptar los métodos para su negocio.

>[!VIDEO](https://video.tv.adobe.com/v/3458040/?learn=on&enablevpops)

## Características destacadas


1. Lógica secuencial y segmentación en Analytics

   * La sesión se centró en técnicas avanzadas para aplicar la lógica secuencial en análisis, haciendo hincapié en la importancia de comprender los puntos de inicio y parada en las secuencias de datos para analizar los comportamientos de los clientes de forma eficaz.
   * Los operadores secuenciales se analizaron como herramientas para identificar patrones como &quot;visita web seguida de visita por correo electrónico&quot; o &quot;envío de solicitudes seguido de sesiones posteriores&quot;.
   * Se resaltó la naturaleza voraz de la lógica de segmento, y se explicó cómo devuelve el conjunto de datos más grande posible a menos que esté restringido por condiciones adicionales.
   * Se introdujeron técnicas para definir el alcance, como secuencias de &quot;solo antes&quot; y &quot;solo después&quot;, para estudiar subconjuntos de datos basados en preguntas comerciales específicas.
   * Se explicó el uso de puntos de comprobación, condiciones de proximidad y criterios de exclusión para refinar el análisis de los datos y responder preguntas comerciales complejas.

2. Gestión de varios puntos de interés en el análisis de datos

   * Andy habló de escenarios en los que los clientes tienen varios envíos de aplicaciones y de la necesidad de analizar los comportamientos después de cada envío en lugar de solo el primero.
   * Se abordaron retos como la superposición de solicitudes y la definición de si se deben incluir o excluir los puntos de interés originales.
   * Se destacó la importancia de aclarar las suposiciones y refinar la lógica para manejar múltiples ocurrencias de una secuencia, lo que garantiza un análisis preciso de los comportamientos de los clientes a lo largo de su ciclo de vida.

3. Técnicas avanzadas para detener la coincidencia de datos

   * La sesión introdujo métodos para detener la coincidencia de datos en puntos de comprobación específicos mediante criterios de exclusión, lo que permitió a los analistas estudiar los datos entre los puntos de inicio y parada definidos.
   * Algunos ejemplos eran el análisis de comportamientos entre &quot;visita web seguida de interacción con aplicaciones móviles&quot; y la detención en &quot;interacción por correo electrónico&quot;.
   * Se explicó el uso de las condiciones &quot;dentro&quot; y &quot;después&quot; para hacer cumplir reglas de proximidad más estrictas y evitar resultados no deseados de la lógica codiciosa.
   * Andy demostró cómo se pueden aplicar estas técnicas para estudiar los comportamientos de los clientes en relación con eventos específicos, como los envíos de aplicaciones.

4. Validación y refinamiento de la lógica de análisis de datos

   * Andy enfatizó la importancia de validar las suposiciones y la lógica de prueba para garantizar resultados precisos, ya que los errores en la creación de segmentos o las suposiciones de datos son comunes.
   * Se compartieron ejemplos de resultados inesperados debido a una lógica ambiciosa, lo que destaca la necesidad de condiciones estrictas como &quot;dentro de un evento&quot; o &quot;dentro de una sesión&quot;.
   * Se recomendaron puntos de referencia de validación, como pequeños conjuntos de datos con características conocidas, para probar y perfeccionar los métodos de análisis.

5. Aplicación de la lógica secuencial a casos de uso en el mundo real

   * Andy proporcionó ejemplos de casos de uso en el mundo real, como el análisis del comportamiento de los clientes después de enviar la solicitud o la identificación de acciones comunes después de compras o revisiones negativas.
   * La sesión demostró cómo la lógica secuencial se puede aplicar a patrones de estudio como &quot;primera sesión después de la aplicación&quot; o &quot;segunda sesión después de la aplicación&quot; en múltiples ocurrencias.
   * Se debatió la importancia de ampliar el análisis a conjuntos de datos más amplios manteniendo al mismo tiempo la precisión, con ejemplos de efectos en cascada en los datos a nivel de sesión.

6. Uso de campos derivados para un análisis flexible

   * Andy presentó el concepto de uso de campos derivados en Adobe Customer Journey Analytics (CJA) para definir momentos de interés de forma dinámica, lo que reduce la necesidad de editar varios filtros para cada análisis.
   * Los campos derivados permiten a los analistas crear filtros relativos a un único campo, lo que permite realizar ajustes rápidos para estudiar diferentes puntos de interés, como aplicaciones específicas de productos u otros eventos de clientes.

7. Aplicaciones prácticas y planes futuros

   * Andy compartió sus planes para la próxima sesión del seminario web, que se centrará en plantillas, hojas de trucos y aplicaciones prácticas de los conceptos discutidos, pasando de la formación a casos de uso procesables.
   * La sesión concluyó con una llamada a la retroalimentación a través de una encuesta para determinar el interés en temas futuros y asegurar la alineación con los objetivos de los asistentes.
   * Andy destacó las microparticipaciones del equipo de Ultimate Success, que ofrece sesiones de formación dirigidas para ayudar a las empresas a aplicar estos conceptos a sus casos de uso específicos.

8. Uso compartido de materiales y acciones de seguimiento

   * Andy confirmó que los materiales del seminario web, incluyendo grabaciones y posts en blogs, serán compartidos con los asistentes, proporcionando una forma documentada del contenido de la sesión.
   * Se animó a los asistentes a ponerse en contacto con sus equipos de administración de etiquetas o CSM para obtener más ayuda y explorar las licencias de Ultimate Success para sesiones de formación personalizadas.
