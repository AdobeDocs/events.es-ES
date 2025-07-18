---
title: 'GEM de AEM: Introducción a CDN administrada por Adobe'
description: Obtenga información sobre cómo configurar la CDN administrada por Adobe en AEM Cloud Service para mejorar el rendimiento y la seguridad con las nuevas funciones de configuración de CDN.
role: Developer, User
level: Intermediate
feature: Edge Delivery Services
doc-type: Event
duration: 3438
last-substantial-update: 2025-01-30T00:00:00Z
jira: KT-17227
exl-id: 4cd0332f-95bf-45f4-a765-aba020c0d7b0
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# GEM de AEM: Introducción a CDN administrada por Adobe

Obtenga información acerca de la CDN administrada por Adobe en AEM Cloud Service y cómo se puede configurar. Únase a nosotros para explorar las nuevas funcionalidades de configuración de CDN que se pueden utilizar para mejorar el rendimiento y la seguridad de sus aplicaciones de AEM as a Cloud Service. En esta sesión descubrirá lo siguiente:

* ¿Qué es la CDN de Adobe?
* Topologías relevantes para AEMaaCS y Edge Delivery Services
* Casos de uso habituales que se pueden implementar con reglas de CDN
* Cómo utilizar RDE para probar e implementar rápidamente configuraciones de CDN

>[!VIDEO](https://video.tv.adobe.com/v/3443168/?learn=on&enablevpops)

*Grabado el 22 de enero de 2025*

¿Tiene una pregunta, tal vez un comentario?  Únase a la conversación en [Experience League Communities](https://adobe.ly/4haufPK).

## Puntos clave

### Funciones clave de CDN administrada por Adobe

* **Dominios y certificados personalizados** esenciales para alojar dominios y certificados personalizados con el fin de establecer conexiones seguras.
* **El almacenamiento en caché** de las respuestas HTTP de la caché es considerablemente más rápido (menos de 10 milisegundos) en comparación con la recuperación del origen (cientos de milisegundos).
* **CDN personalizada y lista para usar** Adobe proporciona una CDN administrada lista para usar, pero los usuarios también pueden traer su propia CDN.

### Opciones de configuración

* **Transformaciones de solicitudes** Modificar encabezados, reescribir rutas, bloquear tráfico y redirigir solicitudes.
* **Filtros de tráfico** Bloquear o permitir el tráfico según reglas específicas.
* **Autenticación** Compatibilidad con clave perimetral, clave de punzonado y autenticación básica.
* **Selectores de origen** solicitudes de proxy a diferentes orígenes en función de reglas definidas.
* **Transformaciones de respuestas** Modificar encabezados y estado de respuesta.

### Implementación y personalización

* **Canalización de configuración** Implementa archivos YAML para configurar reglas CDN.
* **Protección de tráfico** Use reglas de filtro de tráfico para bloquear, registrar y alertar el tráfico según los patrones.
* **Limitación de velocidad** Proteja contra ataques DDoS limitando el número de solicitudes por IP.

### Herramientas y análisis

* **Elasticsearch Kibana Stack** Analice el uso y el tráfico con los paneles proporcionados.
* **Reenvío de registros**: reenvía registros a una instancia de Splunk para su análisis.

### Aspectos destacados de demostración

* **Implementando configuraciones** demostró la implementación de reglas de filtro de tráfico y redirecciones.
* **Selección de origen y autenticación** Mostró cómo configurar la autenticación básica y el tráfico de proxy en orígenes diferentes.

### Prácticas recomendadas

* **Respuestas rápidas** Garantice respuestas rápidas de los orígenes para evitar vulnerabilidades.
* **Buen almacenamiento en caché** Aproveche el almacenamiento en caché para administrar el tráfico de manera eficiente.
* **Use los paneles** para analizar el tráfico y el uso y establecer los límites de velocidad apropiados.
* **Combinar estrategias** Use diferentes estrategias de limitación de velocidad para obtener una mejor protección.
* **Establecer alertas** Reciba una notificación cuando el sitio sea atacado.
* **Reglas de prueba** Comience con las acciones de registro antes del bloqueo para garantizar que las reglas funcionen según lo esperado.

### Contacto y comentarios

* **Comentarios y casos de uso** Póngase en contacto con el equipo para ver casos de uso avanzados y comentarios.
* **Sesiones futuras** Participe en las encuestas para sugerir temas para sesiones futuras.
