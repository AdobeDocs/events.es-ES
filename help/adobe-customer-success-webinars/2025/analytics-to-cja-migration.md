---
title: Prácticas recomendadas para migrar a Adobe Customer Journey Analytics desde Adobe Analytics
description: Conozca los pasos esenciales y las prácticas recomendadas para migrar de Adobe Analytics a Customer Journey Analytics (CJA), incluido el diseño de esquemas XDM, la asignación de datos y la configuración de vistas de datos.
solution: Analytics, Customer Journey Analytics
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
source-git-commit: 90eb4a9d2cf445c58fde776092fb047f820fa207
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Prácticas recomendadas para migrar a Adobe Customer Journey Analytics desde Adobe Analytics

Obtenga información acerca de la migración de Adobe Analytics a Customer Journey Analytics (CJA). Alojada por Nicolina Picone y Maurizio Corò, del equipo de Ultimate Success de Adobe, la sesión ofrece una descripción detallada de CJA, sus funcionalidades y las prácticas recomendadas para la migración.

## Temas clave discutidos

* diferencias entre Analytics y CJA
* la importancia de contar con identificadores de identidad sólidos, alinear estructuras de datos y crear vistas de datos personalizables
* cubre estrategias para importar datos históricos, administrar la atribución de canales de marketing y aprovechar la flexibilidad de CJA para crear informes personalizados

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## Pasos clave

* **Información general de Customer Journey Analytics (CJA)** CJA es una evolución de Adobe Analytics, que se centra en el recorrido completo del cliente en varios puntos de contacto (por ejemplo, móviles, web, CRM, centros de llamadas) en lugar de eventos de seguimiento único. Permite el procesamiento y la manipulación de datos en tiempo real.

* **Preparación para la migración** Los pasos clave para migrar de Adobe Analytics a CJA incluyen garantizar un identificador de identidad seguro (por ejemplo, ID de persona), alinear variables y dimensiones y asignar datos al esquema XDM. Los datos históricos se pueden importar con pasos de validación.

* **Vistas de datos y flexibilidad** CJA permite la creación de vistas de datos personalizables con duraciones de sesión ajustables, filtros de segmentación y configuraciones de atribución. Esta flexibilidad permite generar informes y análisis personalizados.

* **Prácticas recomendadas para la migración histórica de datos** Valide los datos de CJA comparándolos con los datos de Adobe Analytics dentro de un rango aceptable (por ejemplo, una diferencia del 10%). Comience con una breve ventana de relleno (por ejemplo, un mes) y aumente gradualmente.

* **Atribución de canal de mercadotecnia** CJA ofrece capacidades mejoradas para la atribución de canal de mercadotecnia, al eliminar limitaciones como la función &quot;primera página de la visita&quot; y habilitar configuraciones de sesión más dinámicas.
