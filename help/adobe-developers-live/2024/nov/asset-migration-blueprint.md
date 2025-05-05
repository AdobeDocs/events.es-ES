---
title: Modelo de migración de Assets
description: Aprenda a migrar un DAM heredado a Adobe Experience Manager Assets con perspectivas de Achim Koch, que abarcan el análisis de partes interesadas, la planificación de recursos, la transformación de datos y las prácticas recomendadas, como el uso de archivos CSV para la gestión de datos.
feature: Migration
topic: Migration
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1690
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16576
exl-id: f588055b-05c7-44df-be67-799a0e3ee1ed
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Modelo de migración de Assets

Únase a Achim Koch, arquitecto técnico principal en Adobe, para aprender a migrar un DAM heredado a Adobe Experience Manager Assets. Obtenga información sobre el análisis de las partes interesadas, la planificación de recursos, la transformación de datos y las prácticas recomendadas, como el uso de archivos CSV para la gestión de datos. Cree una hoja de ruta para sus propios proyectos de migración de Adobe Experience Manager.

>[!VIDEO](https://video.tv.adobe.com/v/3440442/?learn=on&enablevpops&captions=spa)

## Discusión de comunidad

Continuar la conversación en la [discusión](https://adobe.ly/4hKHpnF) de la comunidad de Adobe Developers Live.

## Puntos clave

* **No hay ninguna herramienta predeterminada para la migración**. No hay ninguna herramienta única que pueda migrar de varios sistemas heredados a Adobe Experience Manager AEM () debido a la diversidad de productos y soluciones personalizadas.

* **Cinco etapas de migración**

   * Planificación de proyectos
   * Planificación de implementación
   * AEM Implementación de
   * Implementación del script de migración
   * Ejecución de migración

* **Participación de las partes interesadas** Es crucial identificar y hacer participar a las partes interesadas, como patrocinadores, usuarios empresariales, administradores de sistemas de TI y soporte de sistemas heredados.

* **Planificación de recursos y cronología** Asegúrese de que los recursos estén disponibles y planifique en función de los días festivos, las horas de mayor actividad y los períodos fuera de los límites.

* **Planificación técnica** Esto incluye el análisis de requisitos, la transformación de datos y la planificación de la infraestructura.

* La migración de **proceso iterativo** implica varias iteraciones de ejecución de scripts, análisis, comentarios y adaptación.

* **Uso de archivos CSV** Los archivos CSV se prefieren por su facilidad de uso y legibilidad durante el proceso de migración.

* **Se recomienda el lenguaje de scripts** Node.js por su compatibilidad con CSV, AWS y HTTP, y por ser una buena oportunidad para aprender JavaScript.

* **Calidad y repetibilidad** Garantice una migración de datos de alta calidad, mantenga los datos originales y los archivos CSV como referencia y repita el proceso.

* **Congelación de contenido** Declare una congelación de contenido durante la migración para evitar que se agreguen nuevos datos después de tomar la instantánea.

* **Herramientas y sugerencias** Use herramientas como código VS con la extensión CSV Rainbow y considere el marcador de orden de bytes (BOM) para los archivos de texto UTF-8.

* **Aprobación empresarial** Reserve tiempo para probar y obtener la aprobación oficial de la empresa después de la migración para eliminar la congelación de contenido.
