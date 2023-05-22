---
title: 'Pregunte a los expertos: extensiones útiles en etiquetas (Launch) para ayudar a cargar de forma adicional el SDK web'
description: ¿Está pensando en migrar su implementación al nuevo SDK web de Adobe?  Analizaremos algunas de nuestras extensiones favoritas en la biblioteca de etiquetas de Adobe, que le ayudarán a llevar la recopilación de datos al siguiente nivel.
solution: Data Collection,Experience Platform
kt: 10528
thumbnail: 346610.jpeg
event-start-time: 2022-08-23 09:00-7
event-cta-url: null
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
source-git-commit: 17070f55bae19ef0751a2c7c536af7758e31affc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Pregunte a los expertos: extensiones útiles en etiquetas (Launch) para ayudar a cargar de forma adicional el SDK web

¿Está pensando en migrar su implementación al nuevo SDK web de Adobe?  Analizaremos algunas de nuestras extensiones favoritas en la biblioteca de etiquetas de Adobe, que le ayudarán a llevar la recopilación de datos al siguiente nivel.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Preguntas y comentarios del programa

### Extensión del asistente de elementos de datos de Evolytics

<br> 
**Pregunta:** Desde el punto de vista de la seguridad de los datos, ¿es seguro utilizar Evolytics, ya que se trata de una extensión de terceros?

**Respuesta:** Sí. Puede revisar el código de extensión si lo desea, además de que no guarda ninguna de las fechas, simplemente realiza una transformación.

<br> 

**Pregunta:** ¿Esto también captura el Adobe de ECID?

**Respuesta:** El ECID de Adobe no se captura dentro de esa extensión. Esta extensión está diseñada para crear identificadores adicionales anónimos (entre otras cosas).

**Respuesta:** Sin embargo, el ECID de Adobe se puede capturar de otras maneras. Compartiremos esto a través de las notas de ExL y Twitter, ya que no podemos compartir enlaces en el chat aquí.

<br> 

**Pregunta:** ¿La funcionalidad hash ofrece varias técnicas de hash como SHA-256 y proporciona claves públicas y privadas?

**Respuesta:** ¡Sip! SHA-256 es la opción predeterminada

<br> 

### Preguntas generales y comentarios:

<br> 

**Pregunta:** ¿En qué hacemos clic para descargar los archivos de origen de las extensiones? ¿Está en el &quot;menú de 3 puntos&quot;?

**Respuesta:** ¡Sí! Los 3 puntos y, a continuación, Descargar origen (desde la vista de catálogo)

<br> 

**Comentario:** Una de las cosas que realmente me gusta de las extensiones es el aspecto que ahorra tiempo de ellas. Muchos de ellos hacen cosas que usted *podría* haga con algún código personalizado, pero con una extensión no es necesario escribir ese código.

**Responder:** Muy bien. Y es repetible sin tener que recrear la rueda cada vez.

<br> 

**Pregunta:** ¿Cómo se admitirán o reemplazarán los complementos de Analytics con las implementaciones de SDK web?

**Respuesta:** Muchos complementos de análisis son realmente innecesarios en estos días gracias a la flexibilidad añadida de las etiquetas de espacio de trabajo y Adobe. Sin embargo, los que no lo están, se están migrando activamente para que los utilice el SDK web.

<br> 

**Pregunta:** ¿Ha habido algún desarrollo en el seguimiento de Activity Map mediante SDK web?

**Respuesta:** Me complace informar de que Activity Map también está trabajando activamente para obtener soporte en el SDK web

<br> 

**Pregunta:** ¿Podríamos tener acceso a la red de Adobe Edge para administrar eventos antes de transferirlos a los destinos finales? Entiendo que también podemos hacerlo en Launch, pero en el futuro, ¿sería posible hacerlo también en el servidor?

**Respuesta:** ¡Sí! Esto es posible a través de nuestra función de reenvío de eventos, que los clientes pueden adquirir a través de cualquiera de nuestros productos de Real-Time CDP (Real-Time CDP Connections, Prime o Ultimate).

**Respuesta:** Conexiones RTCDP (reenvío de eventos) proporciona la capacidad de tener más control antes de enviarlo a destinos que no sean de Adobe.

**Respuesta:** Eche un vistazo a algunos de nuestros otros vídeos en directo de ExL para obtener más información sobre esto (como [este](exl-live-episode-06-23-22.md)).

<br> 

**Comentario:** Llamada rápida para una de mis extensiones favoritas: existe una extensión de tabla de asignación en la que puede leer una tabla para un elemento de datos que &quot;si este valor es este, configúrelo como tal&quot;.

**Responder:** La flexibilidad que ofrecen es bastante impresionante. Tenga en cuenta también que las empresas pueden crear sus propias extensiones privadas, así como si lo desean.

<br> 

**Pregunta:** Mostró los datos individuales de CRM como ciudad y clima, así que ¿dónde almacenamos la respuesta individual?

**Respuesta:** Las respuestas se almacenan en cada evento único que almacena en déclencheur una regla dentro de una propiedad de reenvío de eventos y se utiliza solo en ese evento específico.

<br> 

Continúe la discusión sobre este tema en la [Discusión de la comunidad de Experience League](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## Sesiones adicionales de Experience League en directo de esta serie de recopilación de datos

* [Pregunte a los expertos: aspectos básicos del SDK web](exl-live-episode-05-26-22.md)
* [Pregunte a los expertos - RTCDP Connections](exl-live-episode-06-23-22.md)
* [Pregunte a los expertos: Datastreams y preparación de datos](exl-live-episode-07-21-22.md)
