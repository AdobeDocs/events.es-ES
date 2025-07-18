---
title: Configuración de CDN y WAF en Adobe Experience Manager as a Cloud Service
description: Mejore el rendimiento y la seguridad de las aplicaciones de Adobe Experience Manager as a Cloud Service con reglas de CDN personalizables, protección de WAF y la canalización de configuración, compartidas por los expertos de Adobe.
solution: Experience Manager as a Cloud Service
feature: Security
topic: Performance, Security
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2211
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16574
exl-id: a9f38e79-c707-443d-8b2f-e534ce4dd43d
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Configuración de CDN y WAF en Adobe Experience Manager as a Cloud Service

Desbloquee todo el potencial de la CDN administrada por Adobe con reglas de CDN personalizables, protección de WAF y la canalización de configuración. Marius Petria, científico informático senior de Adobe, Quentin Vecchio, ingeniero de desarrollo de software de Adobe, y Florian Froese, ingeniero de desarrollo de software de Adobe, comparten estrategias para mejorar el rendimiento y la seguridad de las aplicaciones de Adobe Experience Manager as a Cloud Service.

>[!VIDEO](https://video.tv.adobe.com/v/3440605/?learn=on&enablevpops&captions=spa)

## Discusión de comunidad

Continuar la conversación en la [discusión](https://adobe.ly/3O0TyYa) de la comunidad de Adobe Developers Live.

## Puntos clave

* **Introducción a las nuevas funciones de configuración** La presentación presenta nuevas funciones de configuración para la CDN en un servicio en la nube, centrándose en la capacidad de configurar la CDN para varios casos de uso.
* **Opciones de configuración de CDN** Las nuevas opciones permiten la interacción con solicitudes y respuestas HTTP, como agregar o quitar encabezados, reescribir rutas de solicitud, bloquear tráfico, redirigir clientes y realizar proxy a orígenes diferentes.
* **Mejoras de seguridad** Las nuevas funcionalidades incluyen reglas de filtro de tráfico para bloquear o registrar el tráfico según patrones de solicitud, así como la introducción de M WAF para una protección avanzada contra ataques web como inyección de SQL y XSS.
* **Configuración declarativa**: la configuración se realiza utilizando archivos YAML y se implementa mediante una canalización de configuración en Cloud Manager, lo que lo convierte en un proceso rápido y directo.
* **Transformaciones de solicitudes y respuestas** Las nuevas características permiten las transformaciones de solicitudes para normalizar las direcciones URL y quitar parámetros de consulta innecesarios, así como las transformaciones de respuestas para establecer encabezados antes de enviar respuestas a los clientes.
* **Filtros de tráfico y limitación de velocidad** Los filtros de tráfico pueden bloquear IP o países específicos e implementar límites de velocidad para protegerse contra ataques DDoS. La limitación de velocidad se puede configurar en función de varios criterios, como la IP del cliente, el agente de usuario y la ruta de solicitud.
* **Herramientas de monitoreo y análisis** Adobe proporciona herramientas como los paneles de Elasticsearch/Kibana y Splunk para analizar el tráfico y el uso, lo que ayuda a identificar y mitigar posibles amenazas a la seguridad.
* **Demostración práctica** La presentación incluye una demostración que muestra cómo implementar configuraciones de CDN usando Cloud Manager y cómo manejar errores y validar configuraciones localmente usando AEM.
