---
title: Prácticas recomendadas y perspectivas para el modelado de esquemas XDM
description: Modelado de datos maestros en AEP con esquemas XDM, administración de identidades y prácticas recomendadas para una personalización y segmentación escalables y en tiempo real.
topic: Personalization
role: Developer
level: Intermediate
doc-type: Event
duration: 3488
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18019
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Prácticas recomendadas y perspectivas para el modelado de esquemas XDM

En esta sesión, aprenda las prácticas recomendadas y los métodos abreviados esenciales para crear modelos de datos de experiencia (XDM) de Adobe escalables y de alta calidad que se alineen con los estándares de Adobe Experience Platform. Obtenga información sobre la asignación eficaz de la experiencia del cliente y los datos de casos de uso a XDM para una integración perfecta entre Adobe y herramientas externas.

## Puntos de debate

* Cómo definir y organizar componentes XDM para garantizar modelos de datos escalables y flexibles
* Desafíos comunes en el diseño, la evolución y el mantenimiento de XDM

>[!VIDEO](https://video.tv.adobe.com/v/3458042/?learn=on&enablevpops)

## Puntos clave

**Modelado de datos en Adobe Experience Platform (AEP)**

El esquema XDM es la base del modelado de datos en AEP, lo que permite la integración y el uso compartido de datos entre diferentes sistemas. Define la estructura y el significado de los datos, como los atributos de perfil y las acciones basadas en eventos.

**Identity Management**

Una administración de identidad adecuada es crucial para evitar problemas como el colapso del perfil. La función hash de datos confidenciales, como el correo electrónico y el uso de identificadores únicos, pueden ayudar a mantener la integridad de los datos. Se recomiendan los mapas de identidad para la segmentación y personalización en tiempo real.

**Prácticas recomendadas de diseño de esquemas**

Mantenga los esquemas simples y centrados en los casos de uso de marketing. Evite sobrecargar esquemas con atributos innecesarios. Utilice grupos de campos estandarizados y minimice las personalizaciones para la escalabilidad y las pruebas de futuro.

**Evento vs. Atributos de perfil**

Decida si desea modelar los datos como atributos de perfil o eventos en función de objetivos de marketing. Los atributos de perfil son adecuados para la segmentación en tiempo real, mientras que los eventos proporcionan perspectivas históricas para la segmentación basada en el tiempo.

**Gestión de perfiles contraídos y escalabilidad**

Los perfiles contraídos solo se pueden corregir mediante la compatibilidad con Adobe, pero las reglas de gráficos de identidad pueden evitar futuros colapsos. Para reestructurar los esquemas existentes, se recomienda extraer los datos necesarios y empezar de nuevo con un esquema limpio.
