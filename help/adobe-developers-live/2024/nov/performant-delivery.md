---
title: Prácticas recomendadas para la entrega con rendimiento
description: Optimice la entrega y el rendimiento de los medios con Dynamic Media aprovechando el streaming adaptable, los perfiles de vídeo personalizados, las prácticas recomendadas de SEO, la optimización de imágenes, la administración de contenido en lote, los ajustes preestablecidos de visualizador, la invalidación de caché y las imágenes inteligentes.
feature: Dynamic Media, Video, SEO Optimization, Smart Imaging, Viewer Presets, Best Practices
topic: Content Management
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1596
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16572
exl-id: a1920020-b9ce-43be-8f9e-e52aac68da7b
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Prácticas recomendadas para la entrega con rendimiento

Únase a Riya Midha, directora de producto senior de Adobe, para explorar las prácticas recomendadas para configurar Adobe Experience Manager Assets Dynamic Media. Obtenga información sobre cómo optimizar la entrega de recursos, mejorar la transmisión de vídeo, configurar visores y medir y mejorar el rendimiento.

>[!VIDEO](https://video.tv.adobe.com/v/3440420/?learn=on&enablevpops&captions=spa)

## Discusión de comunidad

Continuar la conversación en la [discusión](https://adobe.ly/3YGedpb) de la comunidad de Adobe Developers Live.

## Puntos clave

* **Funciones de Dynamic Media** Dynamic Media permite el envío rápido y flexible de medios personalizados de alta calidad entre dispositivos, con más de 9 billones de envíos de medios al año y volúmenes máximos diarios de hasta 69.000 millones de recursos.
* **Flujo adaptable**: El uso del flujo adaptable para la entrega de vídeo reduce significativamente el almacenamiento en búfer. Una prueba mostró una reducción en el recuento de buffer de 50 a 5 en un vídeo de 60 segundos con un ancho de banda restringido de 5 Mbps.
* **Perfiles de vídeo** La creación de perfiles de vídeo personalizados con codificación de calidad diversa garantiza un rendimiento de vídeo óptimo en diferentes condiciones de red.
* **Prácticas recomendadas de SEO**
   * Utilice conjuntos de reglas para crear direcciones URL descriptivas para mejorar la SEO.
   * Agregue texto alternativo y atributos de título a las imágenes.
   * Utilice imágenes inteligentes y los últimos formatos de imagen como WebP para mejorar las clasificaciones de búsqueda.
* **Optimización de imagen**
   * Utilice parámetros de escala para ajustar la resolución de la imagen según el tamaño de la pantalla.
   * Evite utilizar una calidad de imagen del 100 %; en su lugar, utilice un rango del 80 al 90 % para reducir el tamaño del archivo sin una pérdida de calidad notable.
   * Aplique parámetros de enfoque para mejorar la claridad del texto en las imágenes.
* **Administración de contenido en lotes**
   * Segmente el contenido pensado para la entrega de medios dinámicos de otro contenido.
   * Utilice la sincronización selectiva para optimizar los tiempos de procesamiento y mejorar el tiempo de salida al mercado.
* **Ajustes preestablecidos de visor** Personalice el aspecto y el comportamiento del visor mediante ajustes preestablecidos de visor sin cambios de código. Algunos ejemplos son la edición de botones de reproducción/pausa, la activación de la reproducción automática y el bucle, y la adición de superposiciones de imagen.
* **Invalidación de caché** Use la invalidación de caché para reflejar inmediatamente los cambios realizados en los recursos ya publicados, omitiendo el TTL predeterminado de 10 horas.
* AEM **Supervisión y depuración** Utilice herramientas como la aplicación de escritorio de la aplicación de la consulta y la página del depurador de consultas para rastrear los trabajos de procesamiento e identificar los recursos no procesados.
* **Imágenes inteligentes** Las imágenes inteligentes están habilitadas de manera predeterminada en todos los dominios, lo que reduce el tamaño de los archivos de imagen y mejora los tiempos de carga.
