---
title: Cuentos de 200 trincheras
description: Garantice el éxito del proyecto web priorizando el rendimiento, utilizando Google PageSpeed Insights, optimizando métricas clave como LCP y TBT, administrando los recursos de forma eficiente y siguiendo las prácticas recomendadas para el desarrollo y la optimización de imágenes.
solution: Experience Manager, Experience Manager Sites
feature: Edge Delivery Services
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1321
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16541
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Cuentos de 200 trincheras

Con más de 200 proyectos de Edge Delivery Services completados, Kiran Murugulla, ingeniero sénior de Adobe, y Varun Mitra, arquitecto de Adobe Experience Manager Cloud, comparten las lecciones clave aprendidas. Descubra los secretos detrás de ofrecer experiencias rápidas y de alto rendimiento con elementos vitales web básicos excepcionales.


>[!VIDEO](https://video.tv.adobe.com/v/3439424/?learn=on&enablevpops)

## Discusión de comunidad

Continuar la conversación en la [discusión](https://adobe.ly/4fwWvvi) de la comunidad de Adobe Developers Live.

## Puntos clave

* El rendimiento de **es crítico** El rendimiento, especialmente la velocidad de las páginas web, se destaca como un factor clave para que los proyectos web tengan éxito. Un objetivo principal es garantizar puntuaciones de rendimiento de 100.
* **Prácticas de desarrollo**
   * Utilice Google PageSpeed Insights para realizar pruebas continuas durante el desarrollo.
   * Inicie proyectos con código de repetidor que ya tenga una puntuación de 100 para mantener un alto rendimiento.
   * Asegúrese de que las solicitudes de extracción (PR) cumplen los estándares de rendimiento antes de combinarse.
* **Las métricas clave** se centran en optimizar el Pintado de contenido más grande (LCP) y el Tiempo de bloqueo total (TBT), ya que afectan significativamente las puntuaciones de rendimiento.
* **Administración de recursos**
   * Incluya los recursos necesarios, como fuentes y scripts de terceros, dentro del origen del proyecto.
   * Utilice las fuentes de reserva para mejorar los tiempos de carga.
   * Retrasar la carga de scripts no esenciales para mejorar el rendimiento de carga inicial.
* **Optimización de imágenes**: dé prioridad a la carga de imágenes por encima del pliegue y use la configuración de recuperación de alta prioridad para las imágenes esenciales.
* **Casos prácticos**
   * ***CNN.com***: índices de consultas optimizados y carga retrasada de anuncios de Google para mejorar el rendimiento.
   * ***Herbert Homes*** utilizó la API de observación de intersección para cargar los datos a medida que los usuarios se desplazan, mejorando el rendimiento y la experiencia del usuario.
* **Prácticas recomendadas**
   * Comience con el código de plantillas y utilice un marcado bien estructurado.
   * Utilice selectores CSS avanzados y minimice la manipulación de JavaScript.
   * Céntrese en el desarrollo con prioridad móvil.
   * Asegúrese de que la estructura del contenido sea intuitiva para los autores.
* **Herramientas** Use herramientas como Hojas de cálculo de Google y DSA para rastrear las puntuaciones de rendimiento del sitio a lo largo del tiempo.

