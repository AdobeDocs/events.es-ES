---
title: 'Adobe Pass: nueva API de REST v2'
description: Esta sesión se centra en la introducción de la nueva API REST v2 de Adobe y en guiar a los usuarios a través de su proceso de migración.
role: Developer
solution: Pass
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
exl-id: 745411bb-48d7-4410-a236-d02c2927ac1b
source-git-commit: 088615f28aa91dfd4ba119c11c4c9f8a89441d84
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Adobe Pass: nueva API de REST v2

Esta sesión se centra en la introducción de la nueva API REST v2 de Adobe y en guiar a los usuarios a través de su proceso de migración.

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## Puntos clave destacados

* **Información general y beneficios**

   * La API de REST v2 está diseñada para una autenticación moderna, flexible y escalable, que se adapta a eventos de alta demanda y escenarios de varios dispositivos.
   * Las mejoras clave incluyen cifrado mejorado, coherencia de la sesión, SSO entre dispositivos e información de error extendida para una depuración más rápida.

* **Pasos de migración**

   * Los usuarios deben crear nuevas aplicaciones registradas con ámbitos de la API de REST v2.
   * Las configuraciones existentes, como la identificación de dispositivos y las asignaciones de MVPD, se pueden reutilizar.
   * La migración implica fases como el registro, la configuración, la autenticación, la preautorización y la autorización.

* **Mejoras funcionales**

   * La API RESTful unificada sustituye a los SDK de vecino de Access y simplifica la implementación en todas las plataformas.
   * Compatibilidad con varios perfiles de autenticación dentro de la misma sesión y transiciones entre dispositivos sin problemas.
   * Los flujos de preautorización y autorización siguen siendo obligatorios para el acceso al contenido.

* **Cronología**

   * La API de REST v1 dejará de recibir actualizaciones en diciembre de 2025 y se habrá retirado por completo a finales de 2026.
   * Se recomienda a los usuarios completar la migración mucho antes de estos plazos.

* **Recursos y asistencia**

   * La documentación, los libros de cocina y las preguntas frecuentes están disponibles en Adobe Experience League.
   * Adobe ofrece entornos de zona protegida, tickets de Zendesk y reuniones de migración para obtener asistencia.

* **Aspectos destacados de preguntas y respuestas**

   * La API de REST 2 requiere volver a autenticarse, ya que no es compatible con la versión 1.
   * La preautorización se realiza con fines de interfaz de usuario, mientras que la autorización es necesaria para los tokens de medios.
   * SSO es compatible mediante un nuevo token de servicio de Adobe.
