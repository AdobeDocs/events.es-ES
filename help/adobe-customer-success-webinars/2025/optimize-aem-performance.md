---
title: 'Optimización del rendimiento de AEM: estrategias y técnicas de almacenamiento en caché'
description: La sesión abarcó estrategias y técnicas de almacenamiento en caché, mecanismos y niveles de almacenamiento en caché, administración de contenido dinámico, depuración de problemas de almacenamiento en caché y sincronización de la invalidación de caché entre Dispatcher y CDN.
topic: Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3764
last-substantial-update: 2025-02-21T00:00:00Z
jira: KT-17373
source-git-commit: e7bf8b79ad4920b303fc3afbdfb4adee60614c88
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Optimización del rendimiento de AEM: Estrategias y técnicas de almacenamiento en caché

En esta sesión exploramos varios mecanismos de almacenamiento en caché, como el almacenamiento en caché de páginas, recursos y Dispatcher, así como cómo implementar el almacenamiento en caché a nivel de CDN para optimizar la entrega de contenido y reducir los tiempos de carga. El debate abarcará las prácticas recomendadas para cada capa de almacenamiento en caché, la resolución de problemas comunes y cómo aprovechar las capacidades de CDN para lograr la máxima eficiencia.

## Puntos clave de debate

* Introducción al almacenamiento en caché
* Tipos de almacenamiento en caché, Prácticas recomendadas de almacenamiento en caché, invalidación de la caché y actualización
* Técnicas de depuración

>[!VIDEO](https://video.tv.adobe.com/v/3444452/?learn=on&enablevpops)

## Puntos clave

* **Estrategias y técnicas de almacenamiento en caché** La sesión se centró en varias estrategias y técnicas de almacenamiento en caché para optimizar el rendimiento, incluido el almacenamiento en caché en diferentes capas, como el explorador, la red de distribución de contenido (CDN) y Dispatcher.

* **Mecanismos y niveles de almacenamiento en caché** La discusión abarcó diferentes mecanismos y niveles de almacenamiento en caché, incluyendo el almacenamiento en caché del explorador, el almacenamiento en caché de CDN y el almacenamiento en caché de Dispatcher, y cómo se pueden configurar y administrar.

* **Administración de contenido dinámico** Se analizaron técnicas para administrar contenido dinámico en una página, incluido el uso de Sling Dynamic Include (SDI) y Edge Side Includes (ESI) para garantizar que el contenido dinámico no se almacene en caché mientras que el contenido estático sí se almacena en caché.

* **Depuración de problemas de almacenamiento en caché** Se explicaron varias técnicas para depurar problemas de almacenamiento en caché en diferentes niveles (explorador, CDN, Dispatcher), incluido el uso de encabezados, registros y configuraciones específicas para identificar y resolver problemas de almacenamiento en caché.

* **Sincronización de invalidación de caché** La sesión abordó el desafío de sincronizar la invalidación de caché entre Dispatcher y la red de distribución de contenido (CDN), y recomendó el uso de valores de max-age más cortos y API de purga de CDN para garantizar que ambas cachés se invaliden simultáneamente al activar la página.