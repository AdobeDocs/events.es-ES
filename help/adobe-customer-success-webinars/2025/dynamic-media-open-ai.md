---
title: Dominio de Dynamic Media con API abierta
description: Comprenda las diferencias clave entre Dynamic Media tradicional y el modelo de API abierta, y aprenda a realizar la transición e implementar correctamente Dynamic Media Ultimate con la API abierta.
solution: Experience Manager as a Cloud Service, Experience Manager Assets
feature-set: Experience Manager Assets
feature: SDK/API
topic: Development, Content Management
role: Admin, Developer, User
level: Beginner, Intermediate
doc-type: Event
duration: 2757
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18702
source-git-commit: ef1eacd73c5a4fb9cdfee730d40606ec65bab2a7
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---


# Dominio de Dynamic Media con API abierta

Este seminario web está diseñado para profesionales familiarizados con la versión tradicional de Dynamic Media y que deseen comprender e implementar [Dynamic Media Ultimate](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dm-prime-ultimate) con la API abierta.  Exploraremos el funcionamiento de alto nivel de Dynamic Media Ultimate con la API abierta y lo compararemos con la versión tradicional de Dynamic Media. Nuestro objetivo es proporcionar una comprensión completa de las diferencias entre estos dos enfoques, lo que permite a los participantes familiarizados con Dynamic Media adaptarse fácilmente al modelo de API abierta.

>[!VIDEO](https://video.tv.adobe.com/v/3470620/?learn=on&enablevpops)

## Comparación de funciones clave

| Función | Medios dinámicos | Dynamic Media con OpenAPI |
|-----------------------------|------------------------|----------------------------|
| *Disponibilidad* | On-Premise, AMS, Cloud | Solo nube |
| *Modificadores* | Conjunto enriquecido disponible | Limitado pero en crecimiento |
| *Control de acceso* | Abierto a todos los usuarios | Restringido por funciones |
| *TTL DE CDN* | ~10 horas | ~10 minutos |
| *Aplicación de aprobación* | Publicado automáticamente | Requiere aprobación |
| *Compatible con SEO* | Sí | Sí |

## Escenarios de integración

Estos escenarios de integración demuestran la flexibilidad y escalabilidad de Dynamic Media con OpenAPI para diversas necesidades empresariales.

* **Integración de AEM Sites** Dynamic Media con OpenAPI admite la integración perfecta con AEM Sites, lo que permite recuperar recursos directamente desde el nivel de entrega sin duplicarlos.
* **CMS de terceros** permite la integración con plataformas como Salesforce y Drupal mediante API o aplicaciones micro front-end.
* **Acceso controlado por API** Proporciona API para buscar, recuperar y entregar representaciones optimizadas de recursos.
* **Optimización del nivel de entrega** Assets se sirve a través de Fastly, lo que garantiza una entrega más rápida y eficiente.