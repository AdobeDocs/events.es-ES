---
title: 'Rendimiento de entrega de Adobe Campaign Classic: solución de problemas'
description: En esta sesión se trataron las estrategias clave para mejorar el rendimiento del envío de correos electrónicos y SMS con Adobe Campaign. Abordó desafíos comunes como retrasos de entrega, bajo rendimiento y lentitud transaccional, ofreciendo soluciones como optimización por lotes, registro SQL y monitorización del rendimiento del servidor. Las prácticas recomendadas sobre la capacidad de entrega incluían la autenticación de correo electrónico adecuada (SPF, DKIM, DMARC), la monitorización de listas negras y las comprobaciones de correo no deseado. Para obtener un rendimiento mejorado, los expertos recomendaron flujos de trabajo limpios, reglas de restricción y evitar contenedores compartidos. Sugerencias de envío de SMS centradas en la configuración adecuada de cuentas externas y el análisis de registros. La sesión también hizo hincapié en la validación del seguimiento, el mantenimiento de la base de datos mediante informes de sobreexposición y la aplicación de reglas de presión/fatiga para aumentar la participación. Se compartirá una grabación de sesión por correo electrónico y se publicará en el sitio de Adobe Experience Platform.
version: Classic v7
solution: Campaign Classic v7
product: Adobe Campaign
feature: SMS, Deliverability, Troubleshooting
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2257
last-substantial-update: 2025-04-25T00:00:00Z
jira: KT-17869
source-git-commit: 373605f79b3122382e221252232a26535ff3109b
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---


# Sesiones técnicas: Rendimiento de entrega de Adobe Campaign Classic - Solución de problemas

En esta sesión, exploraremos los desafíos comunes a los que se enfrenta al ofrecer un rendimiento óptimo con Adobe Campaign Classic (ACC) y proporcionaremos estrategias procesables para solucionar y solucionar problemas. Los participantes aprenderán a identificar cuellos de botella en el rendimiento, abordar las incoherencias en la preparación/configuración de la entrega e implementar las prácticas recomendadas para garantizar comunicaciones sin problemas. Desde la optimización de las entregas hasta la superación de las dificultades técnicas, este seminario web equipará a los asistentes con los conocimientos y las herramientas necesarias para mejorar la eficiencia de sus campañas de ACC, impulsar mejores resultados y ofrecer experiencias de cliente de alta calidad.

>[!VIDEO](https://video.tv.adobe.com/v/3457826/?learn=on&enablevpops)

## Puntos clave

**Desafíos y soluciones de entrega**

* Los problemas comunes incluyen retrasos de entrega, errores de preparación, envíos atascados, tasas de éxito bajas, rendimiento bajo, participación baja y lentitud de entrega transaccional.
* Las soluciones implican optimizar el agrupamiento de entregas, monitorizar el rendimiento del servidor, habilitar el registro de consultas SQL, revisar los registros de auditoría y garantizar la correcta configuración de las afinidades de MTA e IP.

**Prácticas recomendadas de envío**

* Garantizar la autenticación de correo electrónico adecuada (SPF, DKIM, DMARC).
* Supervise los estados de lista negra y evite el contenido que active el correo no deseado.
* Utilice comprobaciones de spam para evaluar las puntuaciones de spam antes de enviar correos electrónicos.

**Optimizando el rendimiento de entrega**

* Utilice flujos de trabajo de objetivos limpios y limite los campos de personalización.
* Implemente reglas de restricción, procesamiento por lotes y reglas de topología para exclusiones y filtros.
* Evite compartir contenedores en varios canales para evitar cuellos de botella.

**Resolución de problemas de entrega de SMS**

* Asegúrese de que las cuentas externas estén configuradas de forma exclusiva y de que los procesos de SMS se estén ejecutando.
* Compruebe los registros de SMS para ver si hay errores y las expresiones regulares en la configuración de SMP.
* Póngase en contacto con el proveedor de servicios para problemas de configuración incorrecta.

**Lentitud En La Entrega Transaccional**

* Monitorizar los tiempos de procesamiento internos y totales.
* Asegúrese de que el tamaño de la entrega esté dentro de los límites (60 GB para el lote, 30 GB para el evento).
* Revise las reglas de tipología y la configuración de personalización.

**Seguimiento y participación**

* Valide los flujos de trabajo de seguimiento y los registros del servidor.
* Pruebe fórmulas de seguimiento personalizadas en entornos inferiores antes de la producción.
* Asegúrese de que los servidores de seguimiento estén en funcionamiento.

**Mantenimiento de base de datos**

* Utilice informes de sobreexposición para identificar tablas con sobreexposición alta y justificar un vacío de BD.

**Recomendaciones generales**

* Utilice reglas de presión y fatiga para limitar los correos electrónicos innecesarios.
* Segmente las entregas grandes en lotes más pequeños para optimizar el rendimiento.