---
title: 'Eficiencias de AEM Sites: optimización del rendimiento, configuración y solución de problemas'
description: aspectos básicos de la solución de problemas de Adobe Experience Manager AEM () Sites. AEM Tanto si tiene problemas de rendimiento como si tiene que lidiar con configuraciones complejas, esta sesión le proporcionará habilidades prácticas para mantener y optimizar su entorno de. Priorizaremos las demostraciones en directo sobre las diapositivas, ofreciendo una experiencia práctica para abordar los desafíos del mundo real​Puntos clave de debate:- Configuración del host virtual y asignación de dominios- Problemas de rendimiento- Autorización, Identificación, Permisos de usuario
solution: Experience Manager
version: Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
source-git-commit: 3f245f71cd4db5097b5a9e712114112451d899e4
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Eficiencias de AEM Sites: optimización del rendimiento, configuración y solución de problemas

En este seminario web, profundizaremos en los aspectos básicos de la solución de problemas de Adobe Experience Manager AEM () Sites. AEM Tanto si tiene problemas de rendimiento como si tiene que lidiar con configuraciones complejas, esta sesión le proporcionará habilidades prácticas para mantener y optimizar su entorno de. Priorizaremos las demostraciones en directo sobre las diapositivas, ofreciendo una experiencia práctica para abordar los desafíos del mundo real&#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## Puntos clave

El seminario web se centró en la eficiencia del sitio de AMP, incluida la optimización del rendimiento, la configuración y la resolución de problemas.

### Configuración de Dispatcher

* Importancia de Dispatcher en el envío de sitios web con buen rendimiento.
* Aspectos clave de la configuración de Dispatcher: configuración de host virtual, asignación de dominios con estructura de caché, y creación de informes y redirecciones regulares.

### Rights Management

* Prácticas recomendadas: aplicar derechos a grupos, evitar declaraciones de denegación y evitar una ingeniería excesiva.
* Uso de la herramienta Netcentric ACL para administrar derechos a través de un archivo Yaml, lo que garantiza una implementación y trazabilidad sencillas.

### Problemas de rendimiento

* Importancia de identificar deltas en operaciones de sincronización para evitar vaciados de caché completos.
* Evite las operaciones de página grande durante el horario laboral.
* Simplifique los flujos de trabajo para completar los pasos necesarios.
* Tenga cuidado con los procesos de sistemas de terceros en sistemas de creación, especialmente con herramientas como ImageMagick.
* Evite las solicitudes sincronizadas a sistemas de terceros que no puedan gestionar la carga.
* Administre componentes personalizados pesados para evitar la degradación del rendimiento.
* Supervise las sesiones de larga duración para evitar excepciones de segmentos no encontrados.