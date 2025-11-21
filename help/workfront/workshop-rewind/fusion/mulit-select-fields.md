---
title: Navegación sencilla entre la API de Workfront y los cambios de Fusion para los campos de selección múltiple
description: Obtenga información sobre los próximos cambios de la API de Adobe Workfront y Fusion, incluidas las actualizaciones de campos de selección múltiple, las versiones de suscripción de evento y las estrategias para evitar cambios importantes.
feature: Workfront API, Workfront Fusion, Workfront Integrations and Apps
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3172
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18631
exl-id: 8581b9e5-674b-447a-8a52-1217d197891a
source-git-commit: 48d93e64b075db84d164a743db97fa0202b3e26c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Navegación sencilla entre la API de Workfront y los cambios de Fusion para los campos de selección múltiple

Este taller se grabó el 25 de junio de 2025 y contó con la participación de Andy Hess, que compartió los próximos cambios en la API y Fusion de Workfront.

>[!VIDEO](https://video.tv.adobe.com/v/3469978/?learn=on&enablevpops)

## Recursos

Junto con la grabación bajo demanda, hemos incluido la platina con diapositivas y recursos adicionales:
* [PDF de la diapositiva](https://workfront-experience.s3.us-west-2.amazonaws.com/Training/Guides/Customer+Success+at+Scale/Navigating+the+API+and+Fusion+Changes+for+Multi-Select+Fields+with+Ease+062425.pdf)
* A principios de mayo se organizó un evento en colaboración con el equipo de desarrollo de software de Adobe sobre los cambios en las suscripciones a eventos si desea obtener más información sobre ese área específica, [[Seguimiento de eventos] Preservar los escenarios de fusión durante la actualización de las suscripciones a eventos V2](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/m-p/754182#M4041)

## Información general clave y recursos

* Los cambios en los campos de selección múltiple de la API de Workfront están disponibles en la versión 21 (octubre de 2025) para garantizar un formato de matriz JSON coherente en lugar de respuestas mixtas de cadena/matriz
* Se está introduciendo el control de versiones de suscripción de evento: la versión 2 siempre devolverá campos de selección múltiple como matrices, mientras que la versión 1 mantiene un comportamiento incoherente actual
* Las nuevas suscripciones de evento se establecen automáticamente como predeterminadas en la versión 2 y todas las suscripciones se actualizarán automáticamente a la versión 2 a mediados de enero de 2026
* A finales de este año se lanzará una nueva versión del conector de Workfront con un proceso de actualización manual para conservar la asignación de módulos y evitar cambios importantes
* El asistente de Fusion AI está disponible actualmente, pero requiere un acuerdo de IA firmado y una configuración de licencias adecuada. Si tiene alguna pregunta o está interesado en obtener más información, póngase en contacto con el administrador de su cuenta. [Más información sobre el uso de IA en Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/manage-scenarios/fusion-ai-assistant)
* [Plantillas de Workfront Fusion disponibles actualmente](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/create-and-manage-templates/currently-available-fusion-templates)
* [Llamar a las plantillas de Fusion](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/call-for-fusion-template-ideas/m-p/732085#M3686). Si tienes sugerencias para nuevas plantillas de Fusion, ¡agrégalas aquí! Aquí es donde el equipo extrae ideas  

Si tiene preguntas de seguimiento, responda a esta [publicación comunitaria de Experience League](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-navigating-the-workfront-api-and-fusion-changes/td-p/761253). 

Esperamos verlo en los futuros talleres de éxito del cliente.  No olvide consultar la lista completa de [Eventos de Workfront](https://experienceleague.adobe.com/events/?filters=Workfront) en Experience League y registrarse.
