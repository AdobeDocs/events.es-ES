---
title: 'Optimización de la entrega de contenido: desbloqueo de la potencia de los servicios de Edge'
description: La sesión sobre Edge Delivery Services (EDS) abarcó su arquitectura, integración con la creación basada en documentos y en AEM, creación rápida de sitios, opciones de personalización y prácticas recomendadas para mantener un alto rendimiento.
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
topic: Headless, Integrations, Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
exl-id: 2057e491-9ec3-4bfe-b85a-6b74d70822bf
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# Optimización de la entrega de contenido: desbloqueo de la potencia de los servicios de Edge

En esta sesión, proporcionaremos una descripción general de Edge Delivery Services (EDS) y su arquitectura. Profundizaremos en cómo EDS se integra con la creación basada en documentos y en AEM a través del editor universal. Una demostración en vivo mostrará EDS en acción, seguido de recursos para una exploración más profunda y una sesión de preguntas y respuestas.

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## Principales conclusiones

### Introducción a EDS

* EDS es un conjunto de servicios de composición diseñados para mejorar las capacidades de ATM. &#x200B;
* Su objetivo es ofrecer experiencias excepcionales que impulsen la participación y las conversiones con ciclos de desarrollo rápidos y una puntuación de faro del 100 %. &#x200B;

### Opciones de creación

* **Creación basada en documentos** Utiliza herramientas conocidas como Microsoft Word o Google Docs para la creación de contenido, lo que permite crear contenido rápidamente sin necesidad de mucha formación. &#x200B;
* **Editor universal** Proporciona una interfaz de WYSIWYG similar a los sitios tradicionales de ATM, lo que permite crear contenido visual y más detallado. &#x200B;

### Arquitectura

* EDS se integra dentro del marco de trabajo de Amazon Cloud Service. &#x200B;
* Admite una implementación sin servidor y puede funcionar sin una instancia de autor o editor tradicional. &#x200B;
* Se pueden implementar dos niveles de almacenamiento en caché: en el nivel de infraestructura del cliente y en el nivel de EDS. &#x200B;

### Administración de contenido

* La creación basada en documentos requiere una cuenta de GitHub, Google Drive o Microsoft SharePoint, un complemento de barra de tareas y una herramienta de sincronización de código. &#x200B;
* EDS con creación de IAM requiere una cuenta de GitHub, una licencia de IAM as a Cloud Service y una herramienta de sincronización de código.

### Desarrollo e implementación

* El proceso de creación de un sitio con EDS es rápido, a menudo tarda menos de un día. &#x200B;
* El desarrollo local se puede realizar utilizando el comando aem up para crear una versión local del sitio web.
* Los cambios se pueden confirmar en las ramas de características para probarlos antes de combinarlos con la rama principal. &#x200B;

### Personalización y extensibilidad

* Los componentes personalizados se pueden crear con CSS y JavaScript simples. &#x200B;
* La arquitectura permite integraciones de terceros y fuentes de creación personalizadas.

### Prácticas recomendadas

* Se recomienda utilizar JavaScript y CSS de vainilla para mantener puntuaciones altas en el faro.
* Cualquier introducción de bibliotecas como React debe considerarse y probarse cuidadosamente para evitar la degradación del rendimiento.

### Soporte y documentación

* Hay disponible documentación completa para guiar a los usuarios a través del proceso de configuración y personalización. &#x200B;
* Se recomienda a los usuarios que se pongan en contacto con el servicio de asistencia de Adobe en caso de problemas sin resolver. &#x200B;
