---
title: 'Sesiones técnicas: Subdominio de Adobe Campaign y administración SSL en el Panel de control de Campaign'
description: Obtenga información sobre cómo delegar y configurar subdominios dentro del Panel de control de Campaign de Adobe Campaign, configurar certificados SSL y supervisar la configuración para garantizar la capacidad de envío segura del correo electrónico.
solution: Campaign
feature: Subdomains and Certificates
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3409
last-substantial-update: 2025-09-05T00:00:00Z
jira: KT-18866
source-git-commit: 18ce421793d97372198151afc92b24f3bed053a8
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Sesiones técnicas: Subdominio de Adobe Campaign y administración SSL en el Panel de control de Campaign

En esta sesión, exploramos los conceptos de delegación y configuración de subdominios dentro de Adobe Campaign, incluida la instalación de certificados SSL para proteger los subdominios.

Descubra qué es un subdominio, sus propósitos y los métodos de delegación que permiten a Adobe utilizarlo de forma eficaz. La sesión también cubre los principios de protección de un subdominio a través de certificados SSL y las prácticas recomendadas para mantener un entorno seguro.

Proporcionamos orientación paso a paso sobre la configuración de subdominios mediante el Panel de control de Campaign de autoservicio, resaltando los posibles obstáculos y cómo abordarlos. Los participantes adquieren conocimientos prácticos para garantizar una configuración sin problemas y una administración segura de sus subdominios.

Tanto si es un administrador, desarrollador o propietario de una plataforma, esta sesión le ofrece las habilidades para configurar y proteger subdominios en Adobe Campaign de forma segura.

>[!VIDEO](https://video.tv.adobe.com/v/3471391/?learn=on&enablevpops)

## Dominio de la administración de subdominios en Adobe Campaign

Desbloquee los aspectos básicos de la delegación, configuración y seguridad de subdominios para las comunicaciones por correo electrónico de Adobe Campaign:

* **Delegación de subdominios** Elija entre delegación completa o CNAME para controlar cómo administra Adobe su capacidad de entrega de correo electrónico y DNS.
* **Configuración de DNS y SSL** La configuración correcta de los certificados MX, SPF, DKIM, DMARC y SSL es crucial para el envío de correo electrónico seguro y de buena reputación.
* **Panel de control de Campaign** Utilice la herramienta de autoservicio de Adobe para optimizar la configuración de subdominios, supervisar registros y administrar certificados SSL.
* **Problemas comunes** Evite retrasos y errores al comprender los plazos de auditoría, los requisitos de registro y los pasos para solucionar problemas.

Dominar estos procesos garantiza que sus campañas sean seguras, entregables y mantengan la reputación de su marca.

## Métodos de delegación** completo frente a CNAME

* **Delegación completa** Adobe administra todos los registros DNS del subdominio, lo que garantiza una seguridad y una capacidad de entrega óptimas. Recomendado para la mayoría de los usuarios.
* **Delegación CNAME** El cliente y Adobe comparten responsabilidades DNS. El cliente crea registros CNAME que apuntan a recursos administrados por Adobe.
* **Diferencias clave:
* **Completo** Adobe tiene autoridad total; menos mantenimiento del cliente.
* **CNAME**: responsabilidad compartida; más pasos manuales para el cliente.
* **Sugerencia** Nunca delegue su dominio raíz (solo subdominios) para evitar perder el control sobre su dominio principal.
