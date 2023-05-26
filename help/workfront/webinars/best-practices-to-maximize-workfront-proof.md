---
title: 'Pregunte al experto: prácticas recomendadas para maximizar Workfront Proof'
description: Obtenga información sobre cómo ajustar la configuración, habilitar los buenos informes y evitar escollos comunes en Proof. Este seminario web se grabó el 26 de febrero de 2020.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9916
exl-id: c7333635-834d-4d78-9dea-f64e3205c78a
source-git-commit: ca06e5a8b1602a7bcfb83a43f529680a5a96bacf
workflow-type: tm+mt
source-wordcount: '5566'
ht-degree: 2%

---

# Pregunte al experto: prácticas recomendadas para maximizar Workfront Proof

Aprenda a configurar las opciones de éxito, acceder a las vistas (y otros trucos) para habilitar los buenos informes y comprender cómo evitar escollos comunes en Proof. Este seminario web se grabó el 26 de febrero de 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341122/?quality=12)

## Preguntas y respuestas

**Pregunta**

Actualmente, para que un destinatario pueda compartir una prueba compartida con ellos, debe marcar manualmente la casilla &quot;suscripción&quot; en la configuración de la prueba. ¿Hay algún plan para hacer que esta casilla se marque automáticamente de forma predeterminada?

**Respuesta**

Un administrador puede habilitar/deshabilitar esta opción por defecto para usuarios individuales siguiendo esta ruta: Inicio de sesión en PHQ > Configuración de la cuenta > Usuarios > Haga clic en el nombre del usuario > Configuración de prueba predeterminada.

**Pregunta**

Si no selecciona &quot;Nueva prueba&quot; y carga un documento, el usuario tendrá la opción &quot;Generar una prueba automáticamente&quot;. ¿Puede modificar esta configuración una vez que los archivos ya se han cargado?

**Respuesta**

Sí. Puede ajustar todos los ajustes de prueba seleccionando la prueba en la pestaña Documentos y luego haciendo clic en Detalles de la prueba.

**Pregunta**

¿Esta presentación es aplicable a la herramienta independiente?

**Respuesta**

Recommendations en Funciones de prueba, Alertas de correo electrónico, Opciones de decisión, Reenvío de correos electrónicos y Agrupación/uso compartido/configuración de plantillas de flujo de trabajo son todos relevantes para una prueba independiente.

**Pregunta**

¿Para qué utilizaría una plantilla de prueba?

**Respuesta**

Si el proceso de revisión de contenido de su organización se repite con frecuencia o el contenido lo revisan las mismas personas, puede crear plantillas de flujo de trabajo que contengan los revisores con funciones de prueba y configuraciones de notificación que especifique.

**Pregunta**

¿Qué es una plantilla de flujo de trabajo de prueba?

**Respuesta**

Una plantilla de flujo de trabajo de prueba es una plantilla con un flujo de trabajo de enrutamiento de prueba predeterminado que se puede aplicar a las pruebas. Permiten estandarizar y automatizar los procesos de aprobación de pruebas.

**Pregunta**

¿Cómo se puede crear una plantilla de prueba?

**Respuesta**

Como administrador, deberá seguir esta ruta: PHQ Login > Workflows > New > New Template.

**Pregunta**

¿Permite esa funcionalidad de uso compartido de plantillas compartir con grupos y equipos o solo con usuarios individuales?

**Respuesta**

En este momento no puede compartir plantillas de flujo de trabajo con grupos, equipos, roles o empresas de Workfront. Sin embargo, puede compartirlos con individuos y con Grupos de prueba. Para crear un grupo de prueba, siga esta ruta: PHQ Login > Groups > New Group.

**Pregunta**

Al enviar una prueba, en Organización, ¿hay algún modo de limpiar las carpetas que ve cada usuario para que solo vean las carpetas aplicables a él? ¿En lugar de todas las carpetas que se han realizado dentro de la cuenta de compañías?

**Respuesta**

Esta pregunta está relacionada con Workfront Proof Standalone. Dentro de Workfront Proof independiente puede utilizar carpetas privadas para ocultarlas a usuarios específicos. Esto permite obtener una lista de carpetas más ágil entre las que elegir. Tenga en cuenta que también puede utilizar la lógica de escritura anticipada para localizar la carpeta a la que desea agregar una prueba.

**Pregunta**

¿Los revisores y aprobadores tienen la opción de cambiar esta configuración de notificación?

**Respuesta**

Los administradores de Workfront tienen la capacidad de cambiar la configuración predeterminada de alertas de correo electrónico para usuarios y contactos. Los creadores de pruebas pueden cambiar la configuración de la notificación al crear una prueba, así como en sus pruebas existentes.

Los destinatarios de las pruebas siempre pueden cambiar su alerta de correo electrónico para pruebas específicas en el nivel de prueba dentro de la herramienta Visualizador de pruebas seleccionando el icono Configuración en el menú de la izquierda.

**Pregunta**

¿Las alertas de correo electrónico anulan las notificaciones globales?

**Respuesta**

Las alertas de correo electrónico de prueba son completamente independientes de la configuración global de notificaciones.

**Pregunta**

Si los revisores están configurados como &quot;deshabilitados&quot;, ¿cómo sabrán si hay una nueva prueba para que revisen si han rechazado una anterior?

**Respuesta**

Las alertas de correo electrónico son independientes del correo electrónico de nueva prueba, el correo electrónico de nueva versión, el correo electrónico en riesgo, el correo electrónico tardío y el correo electrónico @Mentions. Si elige &quot;Deshabilitado&quot; como alerta por correo electrónico, solo desactivará las notificaciones sobre actividades como comentarios, respuestas y decisiones en la prueba (con la excepción de los correos electrónicos @Mention de los comentarios).

**Pregunta**

¿La configuración de deshabilitar correos electrónicos es amplia para la empresa? ¿o es por el Portfolio?

**Respuesta**

La configuración ubicada en Configuración > Correo electrónico > Revisar y aprobación que permite/deshabilita el envío de correos electrónicos cuando los destinatarios de prueba realizan comentarios es de ámbito empresarial (es una configuración global).

**Pregunta**

Tengo un usuario &quot;invitado&quot; que se agregó a la prueba y no puedo revisarla. Y el usuario no tiene acceso en Workfront.

**Respuesta**

Si el invitado puede acceder a la prueba, pero no hacer comentarios/decisiones, asegúrese de comprobar su función de prueba en la prueba. En este caso, es posible que se hayan agregado a la prueba con la función de prueba &quot;Solo lectura&quot;. Si están configurados como revisor o revisor y aprobador en la prueba y aún no pueden hacer comentarios, marcas o decisiones, envíe un ticket de asistencia.

**Pregunta**

¿Los usuarios invitados requieren una licencia?

**Respuesta**

Los usuarios invitados no necesitan una licencia.

**Pregunta**

¿No veo el cuadro de decisión de prueba?

**Respuesta**

Si no ve el cuadro de decisión de prueba en una prueba, es posible que esté configurado en la prueba con una función de prueba de solo lectura o revisor, o que aún no se haya iniciado la fase en la que se encuentra en la prueba.

**Pregunta**

¿Puede aclarar la configuración en WF>Configuración: si tiene la opción de enviar un correo electrónico por cada comentario, estos se envían incluso si el correo electrónico en PHQ está deshabilitado? ¿y quién recibe los correos electrónicos??

**Respuesta**

La opción Workfront Setup > Email > Review and Approval notification es independiente de las opciones de Email Alert en el nivel de prueba. Si esta opción está habilitada, todos los usuarios de cada prueba recibirán un correo electrónico cada vez que alguien en las pruebas en las que se encuentren realice un comentario.

**Pregunta**

Anteriormente, recomendaba &quot;deshabilitado&quot; para las alertas de correo electrónico fuera del propietario de la prueba. ¿Seguirán recibiendo los destinatarios una notificación por correo electrónico de que se les ha asignado una prueba en ese caso?

**Respuesta**

Sí. Las alertas de correo electrónico (que pueden configurarse como Todas las actividades, Deshabilitadas, Decisiones, etc.) son independientes de los correos electrónicos de notificación de prueba (Nueva prueba, Nueva versión, Prueba en riesgo, Prueba tardía, @Mentions).

**Pregunta**

¿Qué sucede si tiene una instancia en la que se agrega a alguien a una prueba y cree que no debería estar ahí? ¿No eliminaría &quot;No relevante&quot; y no le daría una opción para elegir?

**Respuesta**

Este es un buen uso para la opción Decisión no relevante. Sin embargo, si alguien no debería estar en la prueba, recomendaría que @Mention al propietario de la prueba en un comentario sobre la prueba y pidiera que lo eliminaran. Si alguien que debe tomar una decisión sobre la prueba toma una decisión de &quot;No relevante&quot; cuando debe tomar una decisión de Aprobado o Cambios requeridos, esto podría alterar el funcionamiento del flujo de trabajo aplicado a esa prueba.

**Pregunta**

¿Dónde puedo encontrar la casilla de verificación para &quot;requerir inicio de sesión&quot; para usuarios invitados?

**Respuesta**

Esto se encuentra dentro de la Configuración de prueba en la Página de Creación de prueba al crear una prueba. Si la prueba ya se ha creado, puede acceder a esta configuración seleccionando la prueba en la pestaña Documentos y haciendo clic en Detalles de la prueba > Configuración. Tenga en cuenta que solo puede compartir las pruebas de Inicio de sesión requerido con personas que tengan una licencia de revisión.

**Pregunta**

¿Puede alguien quitarse de una prueba si alguien más la agregó?

**Respuesta**

Si la persona tiene derechos de edición sobre la prueba a la que se añadió, puede eliminarse. Las personas con derechos de edición serán usuarios de Workfront con una licencia de revisión de nivel de administrador o supervisor, así como personas añadidas a la prueba con funciones de autor o moderador. Cualquier otra persona deberá ser eliminada por alguien con derechos de edición.

**Pregunta**

¿Por qué usaría la aprobación de documentos en lugar de la aprobación de pruebas o viceversa?

**Respuesta**

La aprobación de documento se puede utilizar para un documento que no requiera comentarios ni marcas en línea con el documento que se va a aprobar. Por ejemplo, solo necesito que vea este documento y lo apruebe o lo rechace. Proof permitirá comentarios y marcas dentro del documento en la herramienta Visualizador de pruebas. Por ejemplo, necesito que vea esta prueba, agregue comentarios, agregue marcas y tome una decisión. En el futuro, el plan es unificar las dos funcionalidades, ya que son muy similares.

**Pregunta**

Somos un departamento de marketing y realizamos una aprobación de prueba interna y luego necesitamos enviarla externamente al solicitante. No damos acceso a los solicitantes de nuestros proyectos. Tampoco queremos que vean todos nuestros comentarios en la prueba interna. Ahora estamos haciendo una nueva prueba limpia, la descargamos y se la enviamos por correo electrónico. Queremos que utilicen Proof HQ, pero no estamos seguros de cómo lograrlo sin que también les dé acceso a nuestro proyecto. ¿Alguna sugerencia?

**Respuesta**

Recomendaría utilizar plantillas de flujo de trabajo automatizadas que le permitan utilizar &quot;fases privadas&quot;. Las fases privadas le permiten ocultar los comentarios, las marcas y las decisiones de los revisores invitados en otras fases. Esto permitiría que la revisión de prueba interna se ocultara completamente al solicitante externo.

**Pregunta**

Una vez que otra persona ha creado una prueba, ¿cuál es la mejor manera de agregarse para ser revisor y aprobador?

**Respuesta**

Si es un usuario de Workfront con el permiso de revisión de un administrador o supervisor, puede agregarse como revisor y aprobador a cualquier revisión a la que tenga acceso. De lo contrario, querrá que el propietario de la prueba (o alguien más con derechos de edición de la prueba) le agregue.

**Pregunta**

Hemos intentado etiquetar a los usuarios en una prueba, pero no reciben una notificación por correo electrónico. ¿Hay algo en la configuración de la cuenta para asegurarse de que se envía un correo electrónico?

**Respuesta**

Recomendaría comprobar los filtros de correo electrónico/carpeta de correo no deseado para ver si las notificaciones han llegado allí y luego realizar los ajustes necesarios dentro de la aplicación de correo electrónico para incluir en la lista blanca esos correos electrónicos. También puede ponerse en contacto con nuestro equipo de asistencia para que le ayude.

**Pregunta**

Solo puede @ a alguien si tiene una licencia de revisión, ¿correcto? Como en, esta persona nunca ha estado en la prueba y desea etiquetarla (@).

**Respuesta**

Si es un invitado o un usuario de Workfront con una licencia de revisión de responsable, puede @Mention a cualquiera que esté en la revisión (independientemente de si esa persona tiene una licencia o no). Si es un usuario de Workfront con una licencia de revisión de supervisor o administrador, o es el propietario de la revisión, puede @Mention a cualquier persona de su lista de contactos en la plataforma de revisión.

**Pregunta**

El mayor problema aquí: dirección de correo electrónico %2B (direcciones de correo electrónico duplicadas). ¿Por qué y cómo sucede y cómo se puede remediar?

**Respuesta**

Esto puede ocurrir si alguien agrega manualmente a alguien a una prueba utilizando una dirección de correo electrónico incorrecta. Si encuentra esto, un administrador puede eliminar la dirección de correo electrónico incorrecta de la cuenta de Proof siguiendo esta ruta: PHQ Login > Contacts > Select the wrong email / guest instance > Delete. Si tiene problemas con usuarios que se agregan con direcciones de correo electrónico duplicadas, póngase en contacto con nuestro equipo de asistencia para obtener ayuda.

**Pregunta**

Una vez que se toma una decisión, debe volver a cambiar la prueba a producción. ¿Qué tipo de acceso necesita dar al equipo de producción para que pueda utilizar la acción del comentario si la prueba está bloqueada?

**Respuesta**

Si una prueba está bloqueada, deberá desbloquearla para que las personas puedan responder a los comentarios de acción o a los comentarios. Las personas con los siguientes permisos pueden desbloquear la revisión: El propietario de la revisión, los usuarios de Workfront con un nivel de licencia de revisión de administrador o supervisor.

**Pregunta**

¿Cuál es la mejor solución para que los equipos conozcan las pruebas que ya están en cola de personas?

**Respuesta**

Puede crear un informe de aprobaciones de pruebas dentro de Workfront. A continuación, puede aplicar filtros que solo muestren pruebas para usuarios específicos que aún requieran que se tome una decisión.

**Pregunta**

¿Existe alguna manera de descargar pruebas con sus aprobaciones asociadas en una carpeta?

**Respuesta**

Puede acceder y descargar un informe de resumen de impresión para las pruebas que incluirá todos los comentarios, respuestas, marcas, acciones y decisiones en todas las versiones.

**Pregunta**

Al solicitar que los usuarios tengan acceso a ProofHQ de creación de informes, también se les dará acceso a la sección de la izquierda (por ejemplo, flujos de trabajo, contactos, configuración de cuenta, etc)?

**Respuesta**

Esto dependerá de su nivel de licencia de revisión. Si se configuran con la licencia de responsable o supervisor, podrán acceder a los contactos, pero no podrán acceder a la configuración de la cuenta y a los flujos de trabajo. Si se configuran con la licencia de administrador, tendrán acceso a la configuración de la cuenta y a los flujos de trabajo.

**Pregunta**

En mi organización, el administrador de proyectos envía una solicitud de aprobación a las partes interesadas para que la revisen o formulen comentarios. Ha mencionado que no deberíamos añadir nombres a los campos de Aprobación. ¿Cómo comparte usted, como primer ministro, la prueba creativa con las partes interesadas?

**Respuesta**

El campo Aprobación es para aprobaciones de documentos, que está bien si solo necesita una aprobación de documento simple. Si desea una aprobación de prueba (con comentarios, marcas y una decisión sobre la prueba), querrá agregar a las partes interesadas a la prueba con la función de revisor y aprobador.

**Pregunta**

¿Cómo se agregan personas como nuevas funciones a cualquier prueba que ya se haya creado?

**Respuesta**

Para añadir destinatarios de prueba y seleccionar su función de prueba en una prueba existente, debe seguir esta ruta: seleccione la prueba en la pestaña de documentos > y haga clic en Detalles de la prueba. Cuando se abra la ventana de detalles de la prueba, haga clic en el botón de puntos suspensivos en la parte superior derecha del escenario y seleccione &quot;Compartir&quot;. A continuación, puede añadir los destinatarios y seleccionar su función de prueba y su alerta por correo electrónico.

**Pregunta**

Si concedemos acceso a Proof HQ a los administradores/creadores de pruebas, ¿podemos bloquear las áreas de administración como flujos de trabajo, grupos, etc.?

**Respuesta**

Sí, así lo determina el Permiso de prueba para usuarios. Los usuarios con el permiso de revisión del administrador o el supervisor no tendrán acceso a la configuración de la cuenta ni a las plantillas de flujo de trabajo. Los usuarios con el permiso de revisión del administrador tendrán acceso a Configuración de cuenta y Plantillas de flujo de trabajo. Todos los usuarios con acceso podrán acceder al área de Grupos.

**Pregunta**

¿Cómo pueden los usuarios ver todas las pruebas a las que están asignados sin ser administradores de pruebas?

**Respuesta**

Si un usuario desea ver todas las pruebas sobre las que aún debe tomar una decisión, podrá utilizar el área de Inicio o Mis actualizaciones en Workfront (según su nivel de acceso). También puede crear un informe de Aprobación de pruebas y aplicar filtros para mostrar solo las pruebas de que el usuario que ha iniciado sesión es un revisor y aprobador.

**Pregunta**

Hola: ¿Puede revisar los flujos de trabajo de pruebas automatizadas en situaciones en las que hay tres rondas de diseño y comentarios, y cómo adaptarse a cuando los comentarios se proporcionan tarde y cómo se puede vincular mejor en las tareas de WF para cada ronda (comentarios del diseño y del administrador del proyecto)?

**Respuesta**

Aunque puede adoptar muchos enfoques diferentes para utilizar las tareas junto con la revisión y aprobación. Un enfoque que me gusta adoptar es tener una tarea para el &quot;Enrutamiento de prueba&quot; y utilizar el flujo de trabajo de prueba para administrar las notificaciones a los destinatarios (en lugar de asignarles una tarea). Luego podría crear una tarea para &quot;Ronda de enrutamiento de prueba 2&quot; y &quot;Ronda de enrutamiento de prueba 3&quot; que puede ayudarle a realizar un seguimiento de cuántas rondas se dieron. También podrá realizar un seguimiento del progreso de las pruebas mediante el panel de pruebas (Inicio de sesión PHQ > Panel > Pruebas a administrar). Esta vista indicará el número de pruebas tardías (así como las pruebas en riesgo) que está administrando.

**Pregunta**

Cuando se elimina una prueba, ¿sigue en los servidores una copia de la misma?

**Respuesta**

Sí. Si elimina una prueba que reside en el área de Papelera de la Cuenta de Prueba asociada, se puede restaurar desde allí si es necesario y permanecerá allí hasta que se vacíe la papelera y a menos que se vacíe.

**Pregunta**

¿Hay alguna manera de tener una nueva decisión que activar si el otro usuario rechaza o aprueba con cambios? es decir. El departamento de pruebas ve algo, el gerente del proyecto tendrá que tomar una nueva decisión... incluso si ya la miraron y la aprobaron. (intentando que el administrador de proyectos no tenga que esperar al departamento de corrección de pruebas para realizar su revisión)?

**Respuesta**

Aunque esto no se puede automatizar, puede establecer el Administrador de proyectos con la Alerta de decisiones por correo electrónico. De este modo, cuando el departamento de corrección de pruebas toma su decisión, se notifica al administrador del proyecto la decisión que se tomó y puede volver a la revisión, revisar los comentarios realizados por el departamento de corrección de pruebas y luego cambiar su decisión si es necesario.

**Pregunta**

Por qué cuando marco &quot;Pedir aprobación&quot; cuando envío una actualización en la sección de detalles de la prueba, solo veo el estado SOC y no SOCD. ¿Deberíamos evitar utilizar esta casilla de verificación? Práctica recomendada para enviar una actualización sobre una prueba.

**Respuesta**

Al utilizar la función &quot;Solicitar aprobación&quot;, está trabajando con la funcionalidad de Aprobación del documento, que será independiente de Revisión y de la barra de progreso de SOCD. Si necesita actualizar la función de prueba de un destinatario de prueba, lo que debe hacer es seguir esta ruta: en la pestaña Documents, seleccione la prueba > y haga clic en Proof Details. Cuando se abra la ventana de detalles de la prueba, verá la lista de destinatarios y la opción de la función de prueba (así como las alertas por correo electrónico) se puede ajustar en línea. Esto le permitiría, por ejemplo, cambiar la función de prueba de Revisor a Revisor y aprobador.

**Pregunta**

¿Es posible asegurarse de que los aprobadores finales no tengan acceso a versiones anteriores (y comentarios) si hay en el mismo documento de prueba? ¿Es necesario crear un nuevo documento de prueba o existe una manera de mantener todas las versiones y comentarios en uno y designar el acceso a las versiones?

**Respuesta**

Dentro de Configuración de la cuenta dentro de Prueba puede controlar el acceso compartido/de visibilidad a sus pruebas. Para actualizar esta configuración de modo que los destinatarios de prueba solo vean las versiones de pruebas que usted designe (en lugar de ver todas las versiones de la prueba), deberá seguir esta ruta: PHQ Login > Account Settings > Settings > Sharing > Recipients can view all versions = Disabled.

**Pregunta**

¿Puede añadir la pantalla del panel de prueba como una página externa a un panel WF? ¿Verán el tablero los usuarios que no son administradores?

**Respuesta**

Puede añadir el Tablero de prueba como una página externa dentro de un Tablero. Tenga en cuenta que esto solo lo pueden ver los usuarios con una licencia de revisión.

**Pregunta**

Las funciones de panel e informes de ProofHQ solo están disponibles para los administradores que tienen acceso a Proof, ¿no es así? ¿No son planificadores generales que no tienen acceso de administrador?

**Respuesta**

Esto es correcto. No obstante, puede enviar un caso de soporte con Workfront para solicitar que todos los usuarios con licencia de revisión tengan acceso al sistema de revisión.

**Pregunta**

Hola: Una pregunta sobre la flexibilidad de la propiedad de la prueba: Si se requiere una nueva carga de versión de prueba en ausencia del propietario original, ¿es una práctica recomendada para ellos agregar un compañero al flujo de trabajo como autor y decidirán &quot;No relevante&quot;? (La delegación de la propiedad solo parece funcionar para una sola versión).

**Respuesta**

Este caso de uso y flujo de trabajo funcionarían por completo. Otra cosa que puede considerar, sin embargo, es tener usuarios que puedan necesitar cargar nuevas versiones a pruebas de que no son el propietario, configurados con el Nivel de Permiso de Prueba del Supervisor o Administrador. Este nivel de permiso les permite cargar nuevas versiones en pruebas de las que no son propietarios sin tener que añadirlas a la prueba como autores o moderadores (lo que requiere una decisión).

**Pregunta**

Según tengo entendido, no puede agregar el mismo usuario en etapas posteriores en un flujo de trabajo automatizado, y esto es problemático para nosotros. ¿Se puede modificar para permitir que el mismo usuario se encuentre en varias fases?

**Respuesta**

Aunque no puede agregar un destinatario de prueba a más de una fase de revisión de una prueba, una vez activada la fase de revisión en la que se encuentra, estará en la prueba en las fases restantes de esa versión. Esto les permitiría seguir comentando y respondiendo a los comentarios aunque hayan comenzado otras etapas. La clave para asegurarse de que esto funcione es asegurarse de que no tenga fases bloqueadas cuando se inicien nuevas fases.

**Pregunta**

¿Puede explicar el enrutamiento de pruebas entre etapas? ¿Cómo se puede cerrar uno y pasar a la siguiente etapa?

**Respuesta**

Hay algunas opciones disponibles en las plantillas de flujo de trabajo automatizadas que le permitirán pasar de una etapa a la siguiente. Las opciones que puede utilizar son &quot;Al crear la prueba&quot;, &quot;Cuando todas las decisiones se aprueban en una fase principal&quot;, &quot;Cuando todas las decisiones se aprueban o aprueban con cambios en una fase principal&quot;, &quot;Cuando todas las decisiones se toman en una fase principal&quot; y otras.

**Pregunta**

¿Puede quitar una revisión de un documento que se generó automáticamente, pero no desea que sea una revisión?

**Respuesta**

Si tiene activada la configuración de &quot;Generar automáticamente pruebas al cargar documentos&quot;, no podrá quitar una prueba de un documento. En su lugar, querrá volver a cargarlo con el botón Añadir nuevo > Documentos.

**Pregunta**

¿Puede un usuario decir en la fase 3 del flujo de prueba que se añada otra persona como revisor y aprobador?

**Respuesta**

Si ese usuario tiene derechos de edición sobre la prueba, puede hacerlo. Las personas con derechos de edición serán: El propietario de la prueba, los destinatarios de prueba añadidos a la prueba con la función de prueba de autor o moderador, los usuarios de licencia de prueba con el nivel de permiso de prueba de supervisor o administrador.

**Pregunta**

Si se designa a un usuario como autor, ¿puede este cargar una nueva versión de la prueba? Podría ser alguien distinto del creador de la prueba.

**Respuesta**

Los destinatarios de la prueba con la función de prueba de Autor y Moderador pueden agregar nuevas versiones a las pruebas en las que están con esa función de prueba.

**Pregunta**

Los usuarios externos reciben un correo electrónico por prueba para su revisión. Esto puede ser difícil para ellos rastrear el estado de todas las pruebas que tienen en juego. ¿Hay opciones de paneles o listas de estado de correo electrónico o funciones próximas para que los usuarios externos rastreen su estado en varias pruebas?

**Respuesta**

Recomendaría añadir estos usuarios externos a Workfront con una licencia gratuita de revisor. Esto les permitirá acceder a una página de Mis actualizaciones que incluirá una lista de todas las pruebas pendientes sobre las que tengan que tomar una decisión.

**Pregunta**

¿Puede explicar más sobre las notificaciones de Decisions? ¿Solo recibiré notificaciones con comentarios de prueba de revisores y aprobaciones o también recibiré los comentarios de los revisores y cuándo los recibiré?

**Respuesta**

Las notificaciones de alerta por correo electrónico de decisión solo se envían cuando se toman decisiones sobre la prueba. No se enviarán cuando se realicen comentarios. Sin embargo, si recibe una alerta por correo electrónico de Decisión que indica que un destinatario de la prueba tomó una decisión sobre los cambios necesarios, sabrá que es un buen momento para revisar los comentarios que han agregado (que estarán en la prueba).

**Pregunta**

En cuanto al problema con el reenvío de correos electrónicos, ¿está iniciando sesión como propietario del correo electrónico? ¿Y esto sucedería con entornos bloqueados? ¿Ocurriría con un entorno de SSO?

**Respuesta**

Esto lo registraría en la prueba como la persona que le reenvió el correo electrónico. El uso de Inicio de sesión obligatorio en pruebas y el uso de SSO impedirán que acceda a la prueba como la persona que le reenvió el correo electrónico.

**Pregunta**

¿Dónde puedo acceder al tablero y a los informes de las pruebas?

**Respuesta**

Si tiene un icono de casilla de verificación a la derecha de la barra de búsqueda en Workfront, significa que tiene una cuenta integrada de Workfront y Proof. Al hacer clic en esa casilla de verificación, se le redirigirá a Workfront Proof y la pantalla de inicio será el panel. Los informes se pueden crear con la opción Vistas del panel izquierdo.

**Pregunta**

En la sección &quot;Función&quot;, hay dos marcas de verificación en la parte inferior que mencionan estar a punto de agregar a alguien usando un @mention, etc. En la configuración de Prueba, puede establecer las funciones predeterminadas de cada persona, pero no hay opción de marcar automáticamente esas marcas de verificación, por lo que tendrá que hacerlo cada vez que cree una prueba. ¿Cómo puede convertir esto en predeterminado para un usuario?

**Respuesta**

Actualmente no hay una forma de convertir esto en una configuración predeterminada para los destinatarios de prueba. Sin embargo, puede guardarlos como ajustes predeterminados para los destinatarios en Plantillas de flujo de trabajo automatizadas.

**Pregunta**

¿Cómo cambia a un propietario de prueba?

**Respuesta**

Para cambiar al propietario de una prueba, debe seguir esta ruta: en la pestaña Documents, seleccione la prueba y haga clic en &quot;Proof Details&quot;. Se abrirá la pestaña de detalles de la prueba. Si la persona a la que desea asignar el propietario de la prueba aún no está en la prueba, desea agregarla como destinatario haciendo clic en el botón de puntos suspensivos y seleccionando Compartir. Una vez que la persona se añada a la prueba (o si ya está en la prueba), seleccione su botón de puntos suspensivos correspondiente para seleccionar &quot;Convertir en propietario&quot;. Ahora se les hará propietarios de la prueba.

**Pregunta**

En cuanto a las nuevas versiones de las pruebas... la única manera en que entiendo hacer esto es arrastrar y soltar el archivo sobre el archivo existente. ¿Es esta la forma adecuada de hacerlo?

**Respuesta**

Recomendaría crear nuevas versiones de esta manera: seleccione la prueba en la pestaña Documentos, luego haga clic en el botón Más y elija Nueva versión > Prueba. Esto le llevará a la página Nueva versión, que transmitirá el flujo de trabajo, y le permitirá realizar los ajustes necesarios antes de enrutar la nueva versión.

**Pregunta**

¿Puede deshabilitar los comentarios en las pruebas para compartirlas con un cliente y que no vea todos los comentarios internos del equipo? Para que no tenga que volver a generar una nueva prueba.

**Respuesta**

Recomendaría utilizar plantillas de flujo de trabajo automatizadas que le permitan utilizar &quot;fases privadas&quot;. Las fases privadas le permiten ocultar los comentarios, las marcas y las decisiones de los revisores invitados en otras fases. Esto permitiría que la revisión de prueba interna se ocultara completamente al solicitante externo.

**Pregunta**

¿La fase Workfront Proof solo se añade cuando se utilizan flujos de trabajo automatizados y alguien que no se ha agregado al flujo de trabajo abre la prueba?

**Respuesta**

La fase &quot;Workfront Proof&quot; se añade a las pruebas si un usuario que no es destinatario hace clic en ellas. También se aplicará si alguien convierte una Prueba de flujo de trabajo básico en una Prueba de Workfront automatizada.

**Pregunta**

¿Podemos configurar un flujo de trabajo de prueba en el que se pueda tomar más de una decisión?

Estamos intentando proporcionar informes a nuestro equipo jurídico interno sobre cuándo el asesor jurídico externo ha completado las revisiones de las pruebas (cuántos días, en promedio, tardan en completar la revisión, quién la completa, etc.)

Comenzamos agregando una nueva decisión al flujo de trabajo de prueba llamada &quot;Revisión de OC completa&quot; y pensamos que podíamos crear un informe para rastrearlos.

El problema es que parece que solo se puede tomar una decisión en el flujo de trabajo.

**Respuesta**

Se puede tomar más de una decisión sobre una prueba (sin embargo, solo habrá un estado general en una prueba que provendrá de la decisión sobre la prueba en el peor de los casos) o la decisión tomada por un responsable de la toma de decisiones principal.

Debido a sus requisitos de informes, lo que recomendaría es que todos los usuarios de la prueba utilicen las mismas opciones de decisión (Aprobado, Aprobado con cambios, Cambios requeridos) y luego utilicen los Informes dentro del Panel de prueba (Inicio de sesión PHQ > Informes) y apliquen la opción de filtro para filtrar por destinatarios (incluir los destinatarios de asesoramiento legal externos en el filtro). Entonces podrá ver el tiempo promedio de respuesta en sus pruebas.

**Pregunta**

Una vez arrastrada una nueva versión y soltada en una prueba existente, ¿por qué cambian TODAS las funciones o desaparecen específicamente?

**Respuesta**

Al arrastrar y soltar un documento como una nueva versión, tiene razón en que el flujo de trabajo se elimina de la nueva versión. Si desea conservar el flujo de trabajo de la versión anterior a la siguiente, seleccione la prueba en la pestaña Documentos y, a continuación, haga clic en el botón Más y elija Nueva versión > Prueba. Esto le llevará a la página Nueva versión, que transmitirá el flujo de trabajo, y le permitirá realizar los ajustes necesarios antes de enrutar la nueva versión.

**Pregunta**

Escenario: reenvío de pruebas: es posible que un cliente externo que revise una prueba desee circular internamente en su organización antes de aprobar la prueba. Los demás revisores no estarán necesariamente en el sistema, por lo que no parece que @ en los comentarios funcione. ¿Cuál es el mejor modo de compartirlos? Reenvíe el correo electrónico y señale al destinatario que los comentarios no aparecerán como su nombre.

**Respuesta**

Desea utilizar la funcionalidad Suscripciones de prueba. Esto se puede habilitar en la configuración de la prueba y permite a los destinatarios de la prueba reenviar un vínculo público genérico a la prueba y, a continuación, permitir que las personas se suscriban a la prueba (básicamente, añadiéndose).

**Pregunta**

¿Cuál es una práctica recomendada para utilizar las carpetas de los documentos?

**Respuesta**

Esto dependerá de la naturaleza del proyecto, pero algo que podría considerar es una carpeta de pruebas activa que contenga todas las pruebas/versiones que se enrutan activamente y una carpeta de pruebas aprobadas que contenga todas las pruebas finalizadas y aprobadas. Una vez que la prueba esté totalmente aprobada, debe moverla de la carpeta Pruebas activas a la carpeta Pruebas aprobadas.

**Pregunta**

Si tengo 3 personas en un grupo de críticas, ¿puedo establecer que necesito aprobaciones de 2 de ellas de las 3?

**Respuesta**

Sí. Querrá agregar a las dos personas de las que necesita una decisión como Revisores y aprobadores, y a la tercera persona como Revisor.

**Pregunta**

Queremos enviar una prueba a un cliente externo (que no sea de Workfront) para que la revise y realice comentarios al respecto. Queremos enviarles una prueba clara (en otras palabras, una sin comentarios internos al respecto). ¿Cuáles son los pasos ascendentes correctos para que esto ocurra a fin de garantizar que el cliente externo obtenga la prueba (solo la prueba, sin acceso al propio proyecto) y cómo nos &quot;envían&quot; los clientes externos de vuelta su prueba marcada? Actualmente no utilizamos plantillas de prueba ni flujos de trabajo automatizados.

**Respuesta**

Recomendaría utilizar plantillas de flujo de trabajo automatizado/flujo de trabajo automatizado para esto, ya que le permitirá utilizar la funcionalidad &quot;Fase privada&quot;. Al utilizar la funcionalidad Private Stage, puede hacer que los comentarios/decisiones y los destinatarios de determinadas etapas de revisión permanezcan ocultos para las personas en otras etapas. Por ejemplo, podría tener una fase interna como fase privada y una fase de cliente. Los clientes no podrán ver nada que ver con la fase interna, mientras que usted sí podrá ver la actividad en la fase cliente.

**Pregunta**

¿Es posible mantener a usuarios específicos (también conocidos como correctores) en una etapa temprana sin que se los incluya en bucle en etapas posteriores?

**Respuesta**

Una vez que se añade a una versión de una prueba en una fase, esta permanecerá en esa versión durante las fases restantes. Tiene la opción de bloquear su etapa cuando comience la siguiente (o manualmente), lo que le impedirá hacer más comentarios.

**Pregunta**

¿Dónde podemos ver una lista de todas las personas que han revisado y/o aprobado una prueba, un día qué y a qué hora? Para fines de auditoría, etc. ¿También hay un lugar en el que podamos ver todas las revisiones y aprobaciones de todas las versiones de una prueba?

**Respuesta**

Para ver una lista de la actividad, como cuándo se realizaron los comentarios y las decisiones, querrá hacer clic en Historial de actividades en Detalles de la prueba. Para acceder a esto, siga esta ruta: seleccione la prueba en la pestaña Documentos > Haga clic en Detalles de la prueba > Expanda la sección Actividad. Si desea ver esta información en el nivel de versión, siga esta ruta: Seleccione la prueba en la pestaña Documentos > Haga clic en la pestaña Detalles > Hacia la parte inferior de la pantalla verá una sección Versiones. Desde aquí puede acceder a los detalles de la prueba en el nivel de versión.

**Pregunta**

¿Podría hablar un poco sobre etapas privadas en pruebas?

**Respuesta**

Cuando una fase se convierte en privada, los comentarios y las decisiones no son visibles para las personas que no se agregan a esta fase o que no son supervisores, administradores o administradores de facturación en la cuenta. Además, los revisores que se agregan a una fase privada solo pueden ver la fase a la que se agregan en la prueba y los comentarios realizados en esa fase.
