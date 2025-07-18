---
title: Entornos de desarrollo rápido de Adobe Experience Manager
description: Facilite el desarrollo y la implementación rápidos en entornos de nube con el nuevo SDK de Adobe, reduciendo significativamente el tiempo de implementación y admitiendo actualizaciones rápidas, registros en directo y opciones de configuración avanzadas, como se describe en la vida útil de DevOps 2024.
solution: Experience Manager as a Cloud Service, Experience Manager
feature: Developer Tools
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2427
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16570
exl-id: 330d8be1-14a0-488a-aae0-ee90e1f7621e
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Entornos de desarrollo rápido de Adobe Experience Manager

Explore las prácticas recomendadas para los entornos de desarrollo rápido (RDE) y la consola de desarrollador actualizada. Natalia Angulo Herrera, ingeniera de desarrollo de software en Adobe, y Remo Liechtenstein, ingeniero de desarrollo de software en Adobe, cubren los desafíos de migración, la configuración de AIO CLI, la implementación, las pruebas, el registro y la administración de la configuración para un flujo de trabajo de Adobe Experience Manager más fluido.

>[!VIDEO](https://video.tv.adobe.com/v/3440397/?learn=on&enablevpops)


## Discusión de comunidad

Continuar la conversación en la [discusión](https://adobe.ly/3UJluDo) de la comunidad de Adobe Developers Live.

## Puntos clave

* **Introducción a DevOps Life 2024** La sesión está organizada por Natalia y Remo de Adobe, y se centra en entornos de desarrollo rápido.
* **Declaración del problema** El desafío de los entornos de desarrollo local que funcionan bien localmente pero que fallan cuando se implementan en la nube.
* **Solución** Creación de un nuevo SDK en la nube para facilitar el desarrollo y la implementación rápidos, lo que reduce el tiempo de 30 minutos a segundos o pocos minutos.
* **Proceso de implementación** El nuevo entorno permite actualizaciones y validaciones rápidas a través de un nuevo complemento de API y CLI, lo que permite una retroalimentación e implementación más rápidas.
* **Diferencias de infraestructura** El entorno de nube utiliza una sola instancia de autor y publicación sin alta disponibilidad y no usa MongoDB.
* **Configuración y uso** Los desarrolladores pueden configurar un entorno de desarrollo rápido a través de la interfaz de la nube, usando npm y Adobe IO CLI para la instalación y configuración.
* **Comandos básicos** Los comandos de clave incluyen io amd —help, io login, io status, io install, io history, io delete y io reset.
* **Registro y depuración** El nuevo entorno admite registros activos y el cambio de los niveles de registro sin necesidad de volver a implementarlos, mediante comandos como los registros io am o d.
* **Temas avanzados** Soporte para paquetes front-end y canalizaciones de configuración, lo que permite una implementación e iteración rápidas.
* **Próximas funciones** planea introducir la funcionalidad de instantáneas para facilitar los restablecimientos de entorno y las actualizaciones automáticas sin pérdida de contenido.
* **Preguntas y respuestas y comentarios** La sesión anima a los participantes a unirse al canal de Discord para interactuar en directo y recibir comentarios del equipo de desarrollo.
