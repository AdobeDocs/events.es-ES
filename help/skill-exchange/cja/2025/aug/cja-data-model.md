---
title: 'La arquitectura del análisis: cómo abordar el modelo de datos de Customer Journey Analytics'
description: Aprenda a estructurar los modelos de datos de CJA con jerarquías de eventos, atribución y KPI para desbloquear perspectivas de recorrido del cliente más profundas.
feature: Attribution
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-09-04T00:00:00Z
jira: KT-18813
source-git-commit: 124b52203b98a80dd9202dab1b0dbe575475a52b
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# La arquitectura del análisis: cómo abordar el modelo de datos de Customer Journey Analytics

Un aspecto crucial de la creación de un modelo de datos de CJA es comprender la relación jerárquica entre los diferentes puntos de contacto e interacciones. Esto forma la base para un análisis y perspectivas significativos.

Las consideraciones clave incluyen:

* Identificación y asignación de puntos de interacción del cliente en todos los canales
* Establecimiento de jerarquías y relaciones de eventos claras
* Definición de modelos de atribución coherentes
* Creación de métricas y KPI estandarizados

Al estructurar correctamente estos elementos, las organizaciones pueden rastrear y analizar mejor el recorrido completo del cliente, lo que conduce a perspectivas más procesables y a capacidades mejoradas de toma de decisiones.

>[!VIDEO](https://video.tv.adobe.com/v/3471111/?learn=on&enablevpops)

## Desbloquear el modelado de datos para análisis potentes

Descubra la eficacia de la arquitectura de datos en Adobe Experience Platform (AEP) y Customer Journey Analytics (CJA) para obtener perspectivas procesables y crear informes.

* **El diseño de los esquemas es importante** La elección entre esquemas planos, matrices y matrices de objetos afecta directamente a las capacidades de análisis y a la flexibilidad de los informes.
* **Proceso de transformación** Los datos ingeridos en AEP deben estar cuidadosamente estructurados para garantizar una transformación y un uso ininterrumpidos en CJA.
* **Jerarquía de contenedores** Es crucial comprender los niveles de evento, sesión y persona para el análisis de varios niveles y la creación de informes precisos.
* **Estrategias prácticas** La planificación anticipada, el control de esquemas y el aprovechamiento de las características de la plataforma son esenciales para implementaciones escalables y preparadas para el futuro.

Dominar estos conceptos permite a los equipos optimizar sus flujos de trabajo de análisis y desbloquear perspectivas comerciales más profundas.

## Tipos de esquemas y sus casos de uso

* **Esquemas planos** idóneos para relaciones de datos directas e individualizadas. Ideal para el seguimiento de eventos básico y métricas y dimensiones sencillas.
* **Matrices** útiles para listas de elementos relacionados (por ejemplo, categorías de productos, etiquetas de contenido). Cada elemento de matriz se convierte en una dimensión individual para el análisis.
* **Matrices de objetos** diseñadas para casos de uso complejos, como compras de productos, en los que cada objeto mantiene sus propias propiedades y relaciones. Permite un análisis detallado a nivel de objeto.
* **Elegir sabiamente** Seleccione el esquema más sencillo que satisfaga sus necesidades, pero aproveche las matrices y objetos para escenarios avanzados que requieran preservación de relaciones.