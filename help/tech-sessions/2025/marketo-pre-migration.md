---
title: 'Migración de Marketo a Adobe Admin Console: (antes de la migración)'
description: Adobe está migrando Marketo Engage a Admin Console para mejorar la administración de usuarios. Obtenga información acerca de los tipos de migración automática y automática, los requisitos previos, los cambios posteriores a la migración, las prácticas recomendadas, los problemas comunes y la asistencia. Acceda a la grabación de la sesión en el sitio web de Experience League de Adobe.
solution: Marketo Engage
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 088615f28aa91dfd4ba119c11c4c9f8a89441d84
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Migración de Marketo a Adobe Admin Console: antes de la migración

Únase a nosotros para una migración perfecta a Marketo con expertos en Adobe.

Adelántese a la migración a Marketo con el equipo de identidad y experiencia del cliente de Adobe en este informativo seminario web. Le guiaremos por los pasos clave, las prácticas recomendadas y los desafíos comunes para garantizar una transición sin problemas a Adobe Admin Console.

Lo que aprenderá,

* Una hoja de ruta paso a paso para el proceso previo a la migración
* Prácticas recomendadas para simplificar la transición y evitar problemas
* Respuestas de los expertos a problemas comunes de la migración

Tanto si acaba de iniciar la migración como si se está preparando para los pasos finales, esta sesión le proporcionará los conocimientos y las herramientas necesarias para navegar por el proceso con confianza. No pierda esta oportunidad de seguir adelante y conseguir que su migración a Marketo sea fluida.

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## Puntos clave

### Objetivo de la migración y descripción general

Adobe está migrando Marketo Engage a Admin Console para consolidar todos los productos en un concentrador y mejorar así la administración de usuarios y el acceso a ellos.  Admin Console servirá como centro para administrar los productos de Adobe, las funciones de usuario, los permisos y el acceso a la asistencia. Las URL para acceder a Marketo Engage cambiarán a la plataforma Experience Cloud de Adobe.

### Tipos de migración

* **Migración automática** para organizaciones con menos de 75 usuarios y sin configuración SSL. Adobe se encarga de la migración.
* **Migración automática** para organizaciones con configuración SSL. Los administradores administran el proceso de migración mediante la consola de migración.

### Requisitos previos para la migración

* Los administradores del sistema deben completar el correo electrónico de consentimiento.
* SSL debe configurarse en Admin Console (no en Marketo).

### Cambios posteriores a la migración

* Los usuarios iniciarán sesión con Adobe ID o Federated ID (SSL).
* Los roles de administrador y los permisos determinan los niveles de acceso en Admin Console.

### Prácticas recomendadas

* Compruebe los correos electrónicos de los usuarios y resuelva las cuentas bloqueadas antes de la migración.
* Asegúrese de que se asignan los roles de administrador adecuados.
* Deshabilite los bloqueadores de anuncios o utilice el modo incógnito para evitar problemas de inicio de sesión.

### Problemas comunes

* Los permisos de administración incorrectos pueden limitar el acceso.
* Las extensiones de explorador y los bloqueadores de anuncios pueden interferir con el acceso.
* ADMIN CONSOLE aún no admite la inclusión de direcciones IP en la lista blanca, pero se está desarrollando.

### Impacto en la funcionalidad

* La migración no afectará a los correos electrónicos automatizados, los usuarios de API ni los códigos munchkin.
* La migración afecta principalmente a la autenticación y administración de usuarios.

### Asistencia

* Los usuarios que tengan problemas deben abrir un caso de asistencia con el Servicio de atención al cliente de Adobe.
* Incluya el ID de organización de IMS en los casos de soporte para una resolución más rápida.
