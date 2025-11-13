---
title: Consejos esenciales y prácticas recomendadas para la búsqueda en AEM Lucene
description: Aumente la participación digital con herramientas de búsqueda avanzadas de AEM como filtros, facetas, sugerencias automáticas, NGram y revisión ortográfica. Aprenda de las demostraciones del mundo real.
solution: Experience Manager
feature: Search
role: Admin, Developer
level: Intermediate, Experienced
doc-type: Event
duration: 3630
last-substantial-update: 2025-11-13T00:00:00Z
jira: KT-19550
source-git-commit: 84c9a126769fa94b0197d12ca594137e13edc510
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# Consejos esenciales y prácticas recomendadas para la búsqueda en AEM Lucene

Descubra cómo mejorar su presencia digital y la participación de los clientes con funciones de búsqueda de vanguardia, incluidos filtros, facetas, sugerencias automáticas, NGram y revisión ortográfica. Aprenda de las demostraciones del mundo real y obtenga perspectivas para optimizar sus capacidades de búsqueda con AEM y Lucene. Este seminario web le ofrece la oportunidad de mejorar su experiencia de búsqueda y mantenerse a la cabeza en el panorama digital.

>[!VIDEO](https://video.tv.adobe.com/v/3476410/?learn=on&enablevpops)

## Desbloquear búsquedas potentes en Adobe Experience Manager

Adobe Experience Manager (AEM) aprovecha la búsqueda de Lucene para ofrecer resultados relevantes y rápidos en contenido, recursos y metadatos. En esta sesión se analiza cómo funcionan los índices Lucene, cómo configurarlos y las prácticas recomendadas para maximizar el rendimiento de la búsqueda.

* **Lucene Search está en todas partes**: permite la búsqueda en los portales, el editor y los autores de AEM y gestiona las sugerencias automáticas, los filtros, las facetas y la paginación.
* **Rendimiento de unidad de definiciones de índice** La personalización de las definiciones de índice de Oak es crucial para una búsqueda eficiente y dirigida.
* **Prácticas recomendadas importantes** Copie las definiciones de índice existentes, limite las propiedades indizadas y utilice los indicadores adecuados para las búsquedas de texto completo y propiedades.
* **Funciones avanzadas que mejoran UX** Las facetas, la sugerencia automática, la revisión ortográfica, el aumento y la modificación de secuencias se pueden habilitar para experiencias de búsqueda más enriquecidas.

Comprender estos principios ayuda a garantizar capacidades de búsqueda estables y de alto valor en AEM, lo que respalda los objetivos técnicos y empresariales.

## Bloques de creación del índice Lucene

Las definiciones de índice de AEM Lucene son la base del rendimiento y la precisión de la búsqueda. Los componentes clave incluyen:

* **Tipo** especifica el tipo de índice (Lucene, propiedad, etc.).
* **Restricción de tipo de nodo** Segmenta tipos de contenido específicos (por ejemplo, dam:Asset, cq:Page).
* **Restricción de ruta** Limita la indexación a las rutas de repositorio definidas para mejorar la eficacia.
* **Reglas de agregado**: controla la profundidad y el ámbito del contenido indizado, asegurando que se puedan buscar las propiedades relevantes.
* **Reglas de índice** Configuración principal; establece indicadores como nodeScopeIndex (búsqueda amplia de texto completo) y analyzed (tokenización/normalización).

Una configuración cuidadosa de estos elementos garantiza que las consultas de búsqueda sean rápidas, relevantes y eficientes en términos de recursos.

## Optimización del rendimiento de búsqueda

La optimización eficaz de la búsqueda en AEM Lucene implica la configuración estratégica y el cumplimiento de las prácticas recomendadas:

* **Empiece con los índices existentes** Copie y modifique siempre las definiciones predeterminadas y nunca las genere desde cero.
* **Limitar propiedades indizadas** Solo incluye las propiedades necesarias para mantener los índices limpios y con buen rendimiento.
* **Use Las Banderas Con Sabiduría:
   * **nodeScopeIndex** true para la búsqueda amplia de texto completo
   * **analizado** como verdadero para la tokenización a nivel de propiedad
   * **evaluatePathRestriction** true para consultas basadas en rutas
* **Indexación de propiedades** Prefiere las búsquedas de restricción de propiedades para obtener el mejor rendimiento; use texto completo sólo cuando sea necesario.
* **Ordenar y facetas** Habilite propertyIndex y el orden para ordenar; establezca facet** true para el filtrado basado en el recuento.

La aplicación de estas estrategias conduce a consultas más rápidas, un uso reducido de los recursos y resultados más relevantes.

