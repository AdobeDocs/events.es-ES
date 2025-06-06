---
title: 'Pregunte a los expertos: extensiones útiles en etiquetas (Launch) para ayudar a cargar de forma adicional el SDK web'
description: ¿Está pensando en migrar su implementación al nuevo SDK web de Adobe?  Analizaremos algunas de nuestras extensiones favoritas en la biblioteca de etiquetas de Adobe, que le ayudarán a llevar la recopilación de datos al siguiente nivel.
solution: Data Collection, Experience Platform
feature: Tags
kt: 10528
event-start-time: 2022-08-23 09:00-7
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
duration: 3833
source-git-commit: 0b2f63198af8767f24783dbafd244c9398c24f33
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# Pregunte a los expertos: extensiones útiles en etiquetas (Launch) para ayudar a cargar de forma adicional el SDK web

¿Está pensando en migrar su implementación al nuevo SDK web de Adobe?  Analizaremos algunas de nuestras extensiones favoritas en la biblioteca de etiquetas de Adobe, que le ayudarán a llevar la recopilación de datos al siguiente nivel.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Preguntas y comentarios del programa

### Extensión del asistente de elementos de datos de Evolytics

<br> 
**Pregunta:** Desde el punto de vista de la seguridad de los datos, ¿es seguro usar Evolytics, ya que se trata de una extensión de terceros?

**Respuesta:** Sí. Puede revisar el código de extensión si lo desea, además de que no guarda ninguna de las fechas, simplemente realiza una transformación.

<br> 

**Pregunta:** ¿Esto captura también el ECID en Adobe?

**Respuesta:** El ECID de Adobe no se captura dentro de esa extensión. Esta extensión está diseñada para crear identificadores adicionales anónimos (entre otras cosas).

**Respuesta:** El ECID de Adobe se puede capturar de otras maneras. Compartiremos esto a través de las notas y el Twitter de ExL, ya que no podemos compartir enlaces en el chat aquí.

<br> 

**Pregunta:** ¿La funcionalidad de hash ofrece varias técnicas de hash como SHA-256 y proporciona claves públicas y privadas?

**Respuesta:** ¡Sí! SHA-256 es la opción predeterminada

<br> 

### Preguntas generales y comentarios:

<br> 

**Pregunta:** ¿En qué hacemos clic para descargar los archivos de origen de las extensiones? ¿Está en el &quot;menú de 3 puntos&quot;?

**Respuesta:** ¡Sí! Los 3 puntos y, a continuación, Descargar Source (desde la vista de catálogo)

<br> 

**Comentario:** Una de las cosas que más me gustan de las extensiones es el ahorro de tiempo que suponen. Muchos de ellos hacen cosas que *podrías* hacer con algún código personalizado, pero con una extensión no necesitas escribir ese código.

**Respuesta:** Correcto. Y es repetible sin tener que recrear la rueda cada vez.

<br> 

**Pregunta:** ¿Cómo se admitirán o reemplazarán los complementos de Analytics con las implementaciones de SDK web?

**Respuesta:** Muchos complementos de Analytics no son necesarios en estos días gracias a la flexibilidad agregada de las etiquetas de Adobe y Workspace. Sin embargo, los que no lo están, se están migrando activamente para que los utilice el SDK web.

<br> 

**Pregunta:** ¿Ha habido algún desarrollo en el seguimiento de Activity Map mediante el SDK web?

**Respuesta:** Me complace informar que el Activity Map también está trabajando activamente para obtener soporte en el SDK web

<br> 

**Pregunta:** ¿Podríamos tener acceso a la red de Adobe Edge para administrar eventos antes de transferirlos a los destinos finales? Entiendo que también podemos hacerlo en Launch, pero en el futuro, ¿sería posible hacerlo también en el servidor?

**Respuesta:** ¡Sí! Esto es posible a través de nuestra función de reenvío de eventos, que los clientes pueden adquirir a través de cualquiera de nuestros productos de Real-Time CDP (Real-Time CDP Connections, Prime o Ultimate).

**Respuesta:** Conexiones RTCDP (Reenvío de eventos) proporciona la capacidad de tener más control antes de enviarlo a destinos que no sean de Adobe.

**Respuesta:** Mira algunos de nuestros otros videos de ExL Live para obtener más información sobre esto (como [éste](exl-live-episode-06-23-22.md)).

<br> 

**Comentario:** Llamada rápida para una de mis extensiones favoritas: hay una extensión de tabla de asignación en la que puede leer una tabla para un elemento de datos que dice &quot;si este valor es este, configúrelo como tal&quot;.

**Respuesta:** La flexibilidad que ofrecen es bastante impresionante. Tenga en cuenta también que las empresas pueden crear sus propias extensiones privadas, así como si lo desean.

<br> 

**Pregunta:** Ha mostrado los datos individuales de CRM, como la ciudad y el tiempo, así que ¿dónde almacenamos la respuesta individual?

**Respuesta:** Las respuestas se almacenan en cada evento único que almacena en déclencheur una regla dentro de una propiedad de reenvío de eventos y se utiliza únicamente en ese evento específico.

<br> 

Continúe la discusión sobre este tema en [discusión de la comunidad de Experience League](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620?profile.language=es#M240).
<br> 

## Sesiones adicionales de Experience League en directo de esta serie de recopilación de datos

* [Pregunte a los expertos: aspectos básicos del SDK web](exl-live-episode-05-26-22.md)
* [Pregunte a los expertos - RTCDP Connections](exl-live-episode-06-23-22.md)
* [Pregunte a los expertos: Datastreams y preparación de datos](exl-live-episode-07-21-22.md)

