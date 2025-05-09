---
title: Configuraciones de Dispatcher en Adobe Experience Manager as a Cloud Service
description: Explore las prácticas recomendadas de AEM Dispatcher para el almacenamiento en caché, la seguridad y el rendimiento a fin de maximizar la escalabilidad y la eficacia de AEM as a Cloud Service.
solution: Experience Manager as a Cloud Service
version: Experience Manager as a Cloud Service
feature: Dispatcher
role: Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 4200
last-substantial-update: 2025-05-07T00:00:00Z
jira: KT-17903
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---


# Sesiones técnicas: configuraciones de Dispatcher en Adobe Experience Manager as a Cloud Service

**Adobe Experience Manager (AEM) as a Cloud Service** ofrece escalabilidad, flexibilidad y rendimiento mejorado para plataformas modernas de experiencia digital. En el centro de esta arquitectura se encuentra **AEM Dispatcher**, un componente vital responsable del almacenamiento en caché, la seguridad y la administración de solicitudes. Cuando se configura correctamente, Dispatcher acelera la entrega de contenido, protege los sistemas back-end y aumenta el rendimiento general del sitio.

Esta descripción general resalta la configuración clave de Dispatcher, incluidas las estrategias de almacenamiento en caché, los mecanismos de control de acceso y el filtrado de solicitudes. También se describen las prácticas recomendadas para mantener una implementación segura y de alto rendimiento de AEM en la nube. Tanto si es un desarrollador, arquitecto o responsable de la toma de decisiones empresariales, una comprensión sólida de las configuraciones de Dispatcher es crucial para desbloquear todo el potencial de AEM as a Cloud Service.

>[!VIDEO](https://video.tv.adobe.com/v/3457891/?learn=on&enablevpops)

## Principales conclusiones

* **Dispatcher SDK for Validation**: AEM Dispatcher SDK es una potente herramienta para el análisis estático de configuraciones. Permite una validación rápida de las configuraciones, comprueba la inmutabilidad e identifica errores, lo que ahorra un tiempo significativo en comparación con las implementaciones de canalización completas.

* **Entorno de desarrollo rápido (RDE)** RDE proporciona un entorno de tiempo de ejecución interactivo para probar y depurar configuraciones más allá del análisis estático. Permite una validación y depuración más rápidas, lo que reduce el tiempo necesario para la implementación y las pruebas.

* **Redes avanzadas con proxy Mod** Las configuraciones de red avanzadas, como VPN e IP de salida dedicadas, se pueden configurar mediante Cloud Manager. El módulo de proxy mod permite descargar transacciones de AEM a servicios externos, optimizar el rendimiento y reducir la carga en la JVM.

* **Prácticas recomendadas para configuraciones de Dispatcher** Las recomendaciones clave incluyen el uso de rutas relativas, encabezados x-vhost únicos, encabezados de cliente adecuados y el uso de encabezados de control de caché para administrar el almacenamiento en caché de forma eficaz. Estas prácticas ayudan a evitar errores de canalización y mejorar la eficacia de la depuración.

* **Canalización de nivel web para la implementación** La canalización de nivel web es una utilidad para implementar configuraciones de Dispatcher aisladas. Incluye pruebas adicionales, como la invalidación de la caché, que garantizan que las actualizaciones de contenido se reflejen de forma rápida y precisa en los entornos de producción.