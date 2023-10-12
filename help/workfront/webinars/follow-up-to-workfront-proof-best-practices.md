---
title: 'Pregunte al experto: seguimiento de las prácticas recomendadas de Workfront Proof'
description: Descubra por qué debería utilizar plantillas de flujo de trabajo automatizadas, cómo crearlas y cómo ajustar la configuración de prueba para garantizar la privacidad. Este seminario web se grabó el 4 de marzo de 2020.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9917
exl-id: 2b2f6522-2fd9-4d5e-9bc3-903c1d5e4e3b
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '1638'
ht-degree: 2%

---

# Pregunte al experto: seguimiento de las prácticas recomendadas de Workfront Proof

Descubra por qué debería utilizar plantillas de flujo de trabajo automatizadas, cómo crearlas y cómo ajustar la configuración de prueba para garantizar la privacidad. Este seminario web se grabó el 4 de marzo de 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341123/?quality=12)

## Preguntas y respuestas

**Pregunta**

Parece que nuestra instancia genera automáticamente pruebas al cargar documentos. ¿Hay alguna forma de activar/desactivar esta función?

**Respuesta**

Sí, esta configuración se puede desactivar dentro de su perfil personal. Si hace clic en Mi configuración > Preferencias, hay una casilla de verificación para &quot;Generar automáticamente pruebas al cargar documentos&quot; que se puede seleccionar o anular.

**Pregunta**

¿Puede crear un flujo de trabajo con fases vacías para poder rellenar individuos después de adjuntarlo y permitir que varios equipos utilicen un flujo?

**Respuesta**

Sí, las plantillas de flujo de trabajo automatizadas pueden tener fases en blanco para que, según el equipo que las utilice, se puedan agregar distintos usuarios.

**Pregunta**

En nuestro caso de uso, el diseñador carga el documento, pero el administrador de cuentas genera la prueba y configura el flujo de aprobación. Cuando se necesita una nueva versión, el diseñador agrega la versión solo como documento y el proceso se reinicia. ¿Hay alguna manera de hacer que el administrador de cuentas administre el flujo de prueba y que el diseñador administre el control de versiones sin tener que generar el flujo cada vez que se genera la nueva prueba?

**Respuesta**

Si configura Designer con un nivel de acceso de trabajo o plan en Workfront, se le otorgará una licencia de revisión. Si su licencia de revisión está establecida en Supervisor o Administrator, podrán crear nuevas versiones de pruebas sin tener que realizar el paso manual de hacer que el administrador de cuentas convierta la nueva versión y aplique un flujo de trabajo. La nueva versión solo adoptará el flujo de trabajo de la versión anterior (y también se puede modificar o cambiar en este momento).

**Pregunta**

¿Qué se recomienda para &quot;Alertas por correo electrónico&quot;? decisiones o todas las alertas?

**Respuesta**

Recomiendo que el Creador/Propietario de la prueba esté configurado como &quot;Decisiones&quot; para su alerta de correo electrónico. Recomiendo que todos los demás destinatarios de prueba estén configurados en &quot;Deshabilitado&quot; para sus alertas de correo electrónico (aunque la alerta de correo electrónico esté configurada en Deshabilitado, seguirán recibiendo notificaciones de Nueva prueba, Nueva versión, Prueba tardía y Correo electrónico @Mention). Esta configuración garantiza que las alertas de correo electrónico estén segmentadas y mantiene el correo electrónico al mínimo.

**Pregunta**

¿Puede cambiar el propietario de la prueba a la que se notifica cuando se toman las decisiones? Intentamos utilizar la herramienta de corrección, pero no pudimos cambiar el propietario del documento de la persona que cargó el documento original. Ejemplo: Un administrador de marketing cargó el documento original, pero era un especialista en marketing el que, en última instancia, era responsable de tomar decisiones y realizar cambios.

**Respuesta**

Para cambiar el propietario de la prueba, debe seguir esta ruta: Documents > Select the Proof > Click on &quot;Proof Details&quot; > En la ventana de detalles de la prueba, busque el destinatario que desea que sea el propietario de la prueba > Haga clic en el botón de puntos suspensivos para ese destinatario y elija &quot;Make Owner&quot;.

**Pregunta**

¿Hay algún seguimiento del número de rondas de revisiones que se han producido?

**Respuesta**

Normalmente, las rondas de revisiones coinciden con el número de versiones de prueba.

**Pregunta**

¿Puede una persona estar en más de una etapa? En otras palabras, si tenemos un gerente en un ciclo de revisión temprana que tiene una revisión final en una etapa posterior, ¿cómo lo estableceríamos?

**Respuesta**

Aunque no puede agregar un destinatario de prueba a más de una fase de revisión de una prueba, una vez activada la fase de revisión en la que se encuentra, estará en la prueba en las fases restantes de esa versión. Esto les permitiría seguir comentando y respondiendo a los comentarios aunque hayan comenzado otras etapas. La clave para asegurarse de que esto funciona es asegurarse de que no tiene bloqueos de etapas cuando se inicia la nueva etapa.

**Pregunta**

¿Puede editar los flujos de trabajo existentes?

**Respuesta**

Sí, le interesa ir a Workfront Proof y luego seleccionar Flujos de trabajo en el menú de la izquierda. Aquí puede editar etapas, agregar usuarios, eliminar usuarios, agregar etapas, etc.

**Pregunta**

¿Tiene alguna ventaja específica el hecho de que el flujo de trabajo de aprobación de un documento esté en la prueba en lugar de en la tarea? La tenemos configurada para que esté en la tarea de desarrollo de documento/arte, de modo que SI la ilustración se rechaza en cualquier fase del proceso de aprobación, la tarea vuelve a la acción para que la revise el diseñador asignado. De esa manera, no tenemos que trabajar en dos lugares. PERO, tal vez me estoy perdiendo algo importante acerca de ir por esta ruta.

**Respuesta**

En el caso de las pruebas, se administra el proceso de aprobación mediante el motor de flujo de trabajo de prueba. Esto le permite utilizar la herramienta colaborativa de revisión de pruebas para recopilar comentarios, comentarios, marcas, decisiones y etapas. Tendrá la capacidad de utilizar varios déclencheur de flujo de trabajo para enrutar la prueba y puede utilizar configuraciones únicas para las fases de prueba, como bloqueo, fases privadas o responsables de la toma de decisiones principales. También tiene la opción de asignar funciones de prueba únicas y notificaciones de correo electrónico de prueba únicas. Además, tiene la opción de revisar contenido tan variado como Pruebas estáticas, de vídeo e interactivas (alrededor de 150 tipos de archivos diferentes).

**Pregunta**

¿Quién puede poner el escenario en un escenario privado? ¿Solo administradores?

**Respuesta**

La creación de la plantilla es responsabilidad del administrador, pero cualquier usuario que pueda crear una prueba puede hacer que la fase sea privada.

**Pregunta**

¿La fecha límite se incluye en la notificación por correo electrónico?

**Respuesta**

Sí, si aplica un plazo a una prueba, esto aparecerá en la notificación por correo electrónico.

**Pregunta**

¿Puede compartir una plantilla con un grupo de prueba?

**Respuesta**

Sin embargo, puede tener en cuenta que solo se compartirá con miembros del grupo que tengan licencias de revisión. No podrá compartir plantillas con usuarios o invitados de Workfront que no tengan licencias de revisión.

**Pregunta**

¿Cómo se redirige una prueba al propietario de la prueba si se rechaza?

**Respuesta**

El propietario de la prueba permanece en la prueba durante todas las fases de prueba. Si se rechaza la prueba, no es necesario que la prueba en sí se devuelva al propietario. En su lugar, se notificará al propietario de la prueba por correo electrónico de la decisión tomada, se revisarán los comentarios y se empezará a utilizar una nueva versión.

**Pregunta**

¿Cómo desactivar/ocultar el documento &quot;Descargar&quot; en Proof?

**Respuesta**

Cuando agregue una nueva prueba, querrá desplazarse hasta la parte inferior hasta llegar a Configuración de prueba. Ahí, verá una casilla de verificación para &quot;Descargar archivo original&quot; que puede seleccionar o deseleccionar?

**Pregunta**

¿Cómo afecta esta configuración de privacidad en Configuración de cuenta a la revisión de usuarios que utilizan específicamente la comparación automatizada (en paralelo con la comparación automática)? ¿Impide el revisor comparar dos versiones al configurar de forma predeterminada como Deshabilitado?

**Respuesta**

Para la configuración de uso compartido de &quot;Los destinatarios pueden ver todas las versiones&quot;: si se establece en &quot;Deshabilitado&quot;, si el destinatario no estaba en la versión 1 pero sí en la 2, no podrá comparar las versiones 1 y 2. Tenga en cuenta que los usuarios de Workfront con el nivel de permiso de revisión de Supervisor o Administrator podrán ver todas las versiones independientemente de la configuración.

**Pregunta**

¿Se puede hacer que varias personas carguen una nueva versión? por ejemplo, un redactor sube la versión 1 y luego tenemos el corrector en la etapa 1 . Ven un cambio que debe realizarse, ¿puede la versión de carga 2?

**Respuesta**

Puede hacer que los destinatarios de prueba creen nuevas versiones de pruebas si cumplen los siguientes criterios: 1) Son los propietarios de la prueba (o 2) Se establecen con la función de autor o moderador en la prueba (o 3) Se configuran con el nivel de permiso de prueba de supervisor o administrador).

**Pregunta**

¿Cómo se gestionan varias pruebas (p. ej., A, B y C) con el flujo de trabajo automatizado. ¿Empiezas de nuevo?

**Respuesta**

Puede aplicar una plantilla de flujo de trabajo automatizada a varias pruebas en el momento de crear la versión inicial de las pruebas. Para ello, siga esta ruta: Documentos > Agregar nuevo > Prueba. En la página Nueva prueba, seleccione varios archivos para cargar, aplique la plantilla de flujo de trabajo automatizada y cree las pruebas.

**Pregunta**

¿Se puede exportar una prueba con comentarios a un PDF?

**Respuesta**

Puede exportar un resumen de impresión de una prueba a un archivo de PDF. Contiene todos los comentarios, marcas, respuestas y decisiones.

**Pregunta**

¿Dónde puedo ver la configuración de prueba?

**Respuesta**

Para ver la configuración de prueba en una prueba existente, debe seguir esta ruta: Documentos Pestaña > Seleccionar la prueba > Haga clic en &quot;Detalles de la prueba&quot; > Desde la ventana Detalles de la prueba que se abre, debe expandir el área &quot;Configuración&quot;.

**Pregunta**

¿Puedes etiquetar a alguien en el escenario privado?

**Respuesta**

Si es un destinatario de prueba dentro de la fase privada, podrá etiquetar a cualquier persona dentro de esa fase privada. Si no se encuentra en la fase privada, no podrá etiquetar a alguien desde la fase privada.

**Pregunta**

Una vez activada una fase, ¿puede desactivarla?

**Respuesta**

No podrá desactivar una etapa activa, sin embargo, puede &quot;Bloquear&quot; la etapa, lo que impedirá que las personas dentro de la etapa realicen comentarios y tomen decisiones.

**Pregunta**

¿Qué sucede entre bastidores cuando uno o más revisores de una fase dicen que se requieren cambios? ¿A quién se notifica para cargar una nueva versión?

**Respuesta**

Esto dependerá de la configuración del creador de la prueba o de la &quot;alerta de correo electrónico&quot; de los destinatarios de la prueba. Recomiendo que los creadores/propietarios de pruebas se envíen con la alerta por correo electrónico de &quot;Decisiones&quot;, de modo que se les notifique por correo electrónico cada vez que se tome una decisión sobre la prueba.
