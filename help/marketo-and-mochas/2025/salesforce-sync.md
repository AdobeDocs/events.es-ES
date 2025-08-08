---
title: Marketo & Mochas - Sincronización de Salesforce
description: Domine la sincronización de Marketo y Salesforce con instrucciones expertas sobre permisos, visibilidad de campos, colaboración de administradores y prácticas recomendadas para garantizar una integración optimizada y sin problemas.
feature: Salesforce Integration
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3547
last-substantial-update: 2025-08-07T00:00:00Z
jira: KT-18706
source-git-commit: bc5752512fb1bc50cefe0180c308574e821888a2
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Marketo y Mochas: Sincronización de Salesforce

Marketo tiene muy pocas integraciones nativas, pero Salesforce es la más potente de todas. Con alrededor del 90 % de los clientes de Marketo que también utilizan Salesforce, Adobe se compromete a aconsejar a los clientes sobre cómo teorizar, diagnosticar y optimizar la sincronización entre ambos. La sincronización de Marketo con SFDC se basa principalmente en los permisos de SFDC que se conceden al usuario de sincronización de Marketo. Esto puede resultar difícil para los clientes debido a que varios administradores o equipos diferentes crean silos en la comunicación en torno a las actualizaciones en el sistema.

Este seminario web trata lo siguiente en relación con la sincronización de Marketo &lt;-> SFDC:

· Explicar la vista panorámica de cómo funciona la sincronización
· Ocultar campos y objetos del usuario de sincronización de Marketo en SFDC
· Cómo comunicarse con el administrador de SFDC
· Cómo trabajar de forma eficaz con la asistencia de Marketo
· Aspectos que se deben evitar al sincronizar Marketo con SFDC

>[!VIDEO](https://video.tv.adobe.com/v/3470624/?learn=on&enablevpops)

## Prácticas recomendadas para usar Salesforce Sync

Para utilizar Salesforce Sync con Marketo de forma eficaz, siga estas prácticas recomendadas, explicadas paso a paso en términos sencillos:

1. **Comprender el proceso de sincronización**

   La sincronización conecta Marketo y Salesforce, lo que permite que los datos fluyan entre los dos sistemas. Piense en el &quot;Usuario de sincronización de Marketo&quot; como un puente entre las dos plataformas. Este usuario tiene permisos para leer y escribir determinados datos:

   * **Acceso de escritura** posibles clientes y contactos (Marketo puede actualizarlos en Salesforce).
   * **Acceso de lectura** Cuentas, oportunidades, objetos personalizados y actividades (Marketo puede verlos pero no cambiarlos).

   Cuando los datos cambian en Salesforce o Marketo, la sincronización actualiza el otro sistema cada cinco minutos. Sin embargo, puede priorizar las actualizaciones urgentes mediante pasos de flujo como &quot;Sincronizar con SFDC&quot;.

1. **Limpiar campos**

   Sincronizar solo los campos que se utilizan de forma activa. Por ejemplo:

   * Si tiene campos antiguos como &quot;Notas de la COVID-19&quot; que ya no son relevantes, elimínelos de la sincronización. Esto reduce el desorden y acelera el proceso.
   * Evite sincronizar los campos de fórmula (por ejemplo, &quot;edad de posible cliente en días&quot;) porque no actualizan las marcas de tiempo, lo que puede causar problemas.

1. **Evitar trabajos pendientes**

   El registro de pendientes se produce cuando hay demasiados datos esperando a sincronizarse. Para evitarlo:

   * Limitar actualizaciones innecesarias: por ejemplo, si la puntuación de una cuenta cambia ligeramente (por ejemplo, de 60 a 61), puede almacenar en déclencheur las actualizaciones de todos los contactos relacionados. En su lugar, agrupe las puntuaciones en intervalos (por ejemplo, 0-25, 26-50) para reducir las actualizaciones.
   * Campañas por lotes: utilice campañas por lotes en lugar de campañas de déclencheur para procesar los datos de forma más eficaz.

1. **Administrar errores**

   Pueden producirse errores cuando Marketo intenta actualizar un campo en Salesforce pero no tiene permiso. Para solucionar problemas:

   * Inicie sesión en Salesforce como el usuario de sincronización de Marketo e intente realizar la misma acción. Esto ayuda a identificar problemas de permisos o datos no válidos.
   * Configure campañas recurrentes en Marketo para corregir errores comunes, como estandarizar los valores de país/estado (por ejemplo, &quot;CA&quot; a &quot;California&quot;).

1. **Usar filtros de sincronización personalizados**

   Los filtros personalizados le ayudan a controlar qué registros se sincronizan entre Salesforce y Marketo. Por ejemplo, cree un campo llamado &quot;No sincronizar con Marketo&quot;. Si este campo está marcado como &quot;true&quot; para un registro, no se sincroniza con Marketo. Esto resulta útil para excluir direcciones de correo electrónico no válidas o contactos obsoletos.

1. **Limitar creación de tareas**

   olm Salesforce. Céntrese en actividades significativas como &quot;formulario rellenado&quot; o &quot;vínculo en el que se hizo clic en el correo electrónico&quot;.

1. **Colabore con su administrador de Salesforce**

   Dado que la sincronización implica ambos sistemas, trabaje en estrecha colaboración con el administrador de Salesforce para lo siguiente:

   * Administrar permisos para el usuario de sincronización de Marketo.
   * Limpie los campos innecesarios en Salesforce.
   * Solucionar problemas de sincronización juntos.

1. **Supervisar el rendimiento de sincronización**

   Compruebe con regularidad el estado de la sincronización en la sección de administración de Marketo:

   Busque picos en los paneles &quot;Sincronizar tendencia de registro de pendientes&quot; o &quot;Sincronizar rendimiento&quot;. Esto indica retrasos o actualizaciones excesivas.
Si nota problemas, investigue qué campos o registros están causando el problema.

1. **Usar sabiamente objetos personalizados**

   Los objetos personalizados son estructuras de datos especiales que pueden almacenar información adicional (por ejemplo, detalles del producto). Sincronice únicamente los objetos personalizados necesarios para que las campañas no sobrecarguen la base de datos.

1. **Plan de escalabilidad**

   Al configurar la sincronización, tenga en cuenta lo siguiente a largo plazo:

   * Mantenga un diccionario de datos para rastrear qué campos se sincronizan y por qué.
   * Evite sincronizar campos o registros innecesarios para mantener el sistema eficiente.

Al seguir estos pasos, puede garantizar una integración fluida y eficaz entre Marketo y Salesforce, minimizando los errores y maximizando el valor de los datos.
