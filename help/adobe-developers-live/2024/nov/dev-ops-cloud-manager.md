---
title: Optimización de las DevOps con Cloud Manager
description: Optimizar los flujos de trabajo de implementación con la nueva función "Traer su propio Git" de Adobe en AMP Cloud Manager, lo que permite la integración directa de repositorios Git externos, admite una estrategia de cambio a la izquierda para comprobaciones tempranas de la calidad del código y mejora la eficacia y la adaptabilidad.
solution: Experience Manager, Experience Manager Cloud Manager
feature: Git Repositories, CI-CD Pipeline
topic: Integrations
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1034
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16547
source-git-commit: a5b6c2c3150fcc98686fe74d68f186bfe4e1befa
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---


# Optimización de las DevOps con Cloud Manager

Las prácticas eficientes de DevOps son esenciales para ofrecer experiencias a escala. Adrian Tanase, ingeniero de desarrollo de software en Adobe, explora cómo Adobe Experience Manager Cloud Manager puede optimizar los flujos de trabajo de implementación, mejorar la automatización y admitir la integración y el envío continuos (CI/CD).

>[!VIDEO](https://video.tv.adobe.com/v/3439904/?learn=on&enablevpops)

## Discusión de comunidad

Continuar la conversación en la [discusión](https://adobe.ly/3Ywf7Vm) de la comunidad de Adobe Developers Live.

## Puntos clave

* **Presentación de una nueva característica** Adriana Clayton de Adobe presentó una nueva característica en AMP Cloud Manager llamada &quot;Trae tu propio Git&quot;.
* **Propósito de la característica** La característica está diseñada para optimizar los flujos de trabajo de implementación, de modo que sean más rápidos, eficientes y adaptables a los proveedores preferidos.
* **Desafíos resueltos**: la función aborda la complejidad de sincronizar repositorios Git externos con repositorios Git de Adobe, lo que agrega pasos y tiempo adicionales al proceso de implementación.
* **Solución proporcionada** &quot;Traer su propio Git&quot; permite la conexión directa de repositorios Git externos públicos y privados a canalizaciones Cloud Manager, lo que permite la percepción inmediata de los cambios del código y la ejecución de acciones antes de la combinación del código.
* **Estrategia Mayús Izquierda** La integración admite una estrategia Mayús Izquierda, que permite ejecutar las comprobaciones de calidad del código antes en el proceso de desarrollo y proporcionar comentarios oportunos a los desarrolladores.
* **Demostración y validación** Se proporcionó una demostración que muestra cómo integrar repositorios y validarlos mediante Cloud Manager, incluidos los pasos para los repositorios de GitHub y Bitbucket.
* **Impacto del cliente** Desde su disponibilidad general, más de 130 clientes han incorporado sus repositorios, lo que ha impedido que más de 2500 solicitudes de extracción con problemas de calidad del código lleguen a la producción.
* **Mejoras futuras** planea expandir la función para incluir informes directamente en GitLab y Bitbucket, y extender &quot;Trae tu propio Git&quot; a los servicios de envío Edge para obtener más flexibilidad.
* **Animación para recibir comentarios** Se recomienda a los clientes que proporcionen comentarios y participen en la fase de adopción anticipada de repositorios que no sean de GitHub.
