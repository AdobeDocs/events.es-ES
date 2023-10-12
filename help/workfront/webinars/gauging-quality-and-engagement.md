---
title: Pregunte al experto - Medición de la calidad y la participación
description: Aprenda a crear informes que respondan a preguntas de calidad y participación. Este seminario web se grabó el 13 de noviembre de 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9914
exl-id: 76a8e418-71c7-414a-9938-e64e4e73c184
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 1%

---

# Pregunte al experto - Medición de la calidad y la participación

Aprenda a crear informes que respondan a preguntas de calidad y participación. Este seminario web se grabó el 13 de noviembre de 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Preguntas y respuestas

**Pregunta**

Hay algunos campos por los que se puede filtrar, pero que no están disponibles cuando intenta agrupar por ellos. ¿Está trabajando para que sean opciones coherentes?

**Respuesta**

Las herramientas de creación de informes no le permitirán agrupar por un campo dinámico o uno que pueda tener varias opciones seleccionadas a la vez, como un campo de casilla de verificación. Solo puede agrupar campos que tengan un solo valor, aunque tengan muchas opciones.

Puede filtrar por casillas de verificación y verlas; simplemente, no puede agruparlas.

**Pregunta**

En el ejemplo de la iteración en los roles, ¿puedo mostrar el principal en negrita?

**Respuesta**

En la iteración podemos identificar el rol principal. Es necesario hacerlo en una expresión de valor, pero los códigos HTML no se reconocen en una expresión de valor. Así que necesitamos encontrar otra manera de identificar el rol como el principal. Pongo &quot;**&quot; antes y después del nombre de rol principal en este código. Pruébalo y mira cómo te gusta:

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

Esto le proporcionará una lista como esta:

```
Support Engineer 
QA Engineer 
**Designer**
```

Donde Designer es la función principal de este usuario.

**Pregunta**

¡Hola! Estoy creando un flujo de trabajo para nuestro equipo editorial que lleva un registro de dónde se encuentra un artículo en su ciclo de vida (redacción inicial —> revisiones de departamento(s) —> ediciones finales —> publicación). Quieren ver fácilmente en qué hito o tarea se encuentra actualmente. Los comentarios que obtengo son que la vista de Hito estándar (con el sombreado rojo o verde) es demasiado &quot;ocupada y compleja&quot;. ¿Hay alguna forma de mostrar simplemente el &quot;Nombre del proyecto&quot; y el &quot;Hito actual&quot; en una tabla o cuadrícula?

**Respuesta**

Sí. Puede crear un informe de tareas que muestre las tareas de hito en las que se está trabajando actualmente y con qué tarea está asociado. Puede hacerlo en una tabla o en un informe de lista.

**Pregunta**

¿Se puede combinar la información de prueba con la información del proyecto en un informe?

**Respuesta**

Si ha creado un informe de Aprobación de pruebas, la información del proyecto se puede extraer a columnas mediante el modo de texto. Por ejemplo, si desea hacer referencia al nombre del proyecto en una columna, puede utilizar lo siguiente:

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**Pregunta**

También me gustaría más información sobre los informes de datos de prueba en relación con el proyecto. Por ejemplo, un informe de proyecto que incluya una decisión sobre la prueba y comentarios.

**Respuesta**

Para hacer referencia a la información del proyecto y a la información de la prueba en un solo informe, debe crear un informe de Aprobación de la prueba. Actualmente, los comentarios de una prueba no se pueden incluir en este informe. Sin embargo, cada decisión de aprobador de prueba se puede encontrar en su propio elemento de línea, en la columna Decisión del aprobador.

**Pregunta**

Uso sharecol a menudo para crear un solo estado de página (muchas columnas). Sin embargo, encuentro que si después de crear un informe quiero agregar una columna en la parte superior de la página, es muy largo volver atrás y modificar. ¿Tiene consejos o trucos para realizar este tipo de cambio?

**Respuesta**

Si está hablando de colocar una columna en la parte superior de una lista de columnas en modo de texto, solo necesita volver a numerar las columnas manualmente.

Pero si ya ha creado el informe con la primera columna como algunas columnas compartidas y desea colocar otra columna compartida en la parte superior de la lista, esto es más fácil.

En el editor de informes solo tiene que añadir un par de columnas nuevas y arrastrarlas al extremo izquierdo de la pantalla Columnas (Ver). después de hacer esto, eche un vistazo a lo que solía ser la columna izquierda y verá que los números de columna del modo texto se han incrementado. Arrastre tantas columnas en blanco como necesite. Asegúrese de colocar algo en esas columnas en blanco antes de guardarlo o, de lo contrario, se eliminarán.

**Pregunta**

Hola, con respecto al informe final de errores, ¿cómo se pueden realizar los informes para varios proyectos si hay errores para varios proyectos??

**Respuesta**

Puede filtrar por portafolio o proyecto, dependiendo de cómo haya organizado su trabajo.

También puede filtrar en colas de solicitudes. Es posible que desee configurar colas de solicitudes para cada proyecto en el que puede crear usuarios de clientes como revisores que puedan iniciar sesión y enviar tickets directamente a las colas de solicitudes que ha compartido con ellos.

**Pregunta**

Los primeros informes se basaban en proyectos o nombres de proyectos. ¿Se puede hacer esto también en tareas? Si es así, ¿cuál es la mejor manera de agruparlas?, ya que posiblemente el nombre de la tarea sería diferente con más frecuencia que no... ¡gracias!

**Respuesta**

Todos estos informes se pueden realizar como informes de tareas, problemas o proyectos, según cómo decida realizar el seguimiento de las cosas.

Una forma habitual de agrupar tareas sería agruparlas primero por el nombre de su proyecto y, a continuación, por el nombre de la tarea dentro de cada proyecto. De este modo, si tiene dos tareas con el mismo nombre, es fácil ver en qué proyecto se encuentran.

**Pregunta**

Quiero saber cuáles son las pruebas pendientes, a qué tarea y proyecto están vinculados, cuándo se enrutó, cuándo vence y quién es el moderador y el aprobador.

**Respuesta**

Las pruebas pendientes se pueden filtrar esperando una decisión > Es igual a > Verdadero dentro de un informe de aprobación de pruebas. Hay una columna para Aprobador, que le dirá quién aún no ha tomado una decisión.

Puede hacer referencia a la tarea o al proyecto al que está vinculada la prueba mediante el modo de texto (vea los ejemplos siguientes).

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name
valueformat=HTML
```

En cuanto a la fecha de enrutamiento, la fecha de vencimiento y el moderador, actualmente esos campos no se pueden extraer en ninguno de los informes de Workfront, por lo que debería hacer clic en Proof directamente para ver esa información.

**Pregunta**

¿Puede configurar un formulario personalizado para enviar automáticamente a un solicitante una vez completada su solicitud? ¿Cómo una encuesta de &quot;satisfacción del cliente&quot;?

**Respuesta**

Aquí hay una cosa que puede hacer que satisfaga sus necesidades. Puede adjuntar una notificación de recordatorio a un problema que enviará un correo electrónico al campo &quot;Ingresado por&quot; después de que se haya ingresado una fecha real de finalización. Ingresado por es la persona que creó el problema.

Podría crear la notificación de recordatorio como lo hicimos en el seminario web para &quot;Recordatorio para rellenar la revisión después de la acción (AAR)&quot;, excepto que este sería un recordatorio de problema. Probablemente quiera crear también una plantilla de correo electrónico para ella a fin de proporcionar un vínculo a la encuesta. Deberá aplicar la notificación de recordatorio manualmente a cada problema (o utilizar la edición masiva).

Una integración sería mejor, ya que podría automatizar los pasos manuales, pero la notificación de recordatorio se puede realizar de inmediato.

**Pregunta**

He creado un informe que muestra los proyectos por tipo de plantilla. Puedo enumerar el propietario del proyecto, pero no las personas asignadas a un proyecto.

**Respuesta**

Si desea extraer el equipo del proyecto (pestaña Asignación de personal) a una columna dentro del informe del proyecto, deberá crearlo en modo de texto. El modo de texto es el siguiente:

```
displayname=Staffing 
listdelimiter=<p> 
listmethod=nested(projectUsers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

## Código de modo de texto para el informe de participación de AAR

```
column.0.displayname=Task Details
column.0.value=<b>Project Name:</b>&nbsp;
column.0.valueformat=HTML
column.0.sharecol=true
column.1.valuefield=project:name
column.1.valueformat=HTML
column.1.sharecol=true
column.2.value=<br>
column.2.valueformat=HTML
column.2.sharecol=true
column.3.value=<b>Task Name:</b>&nbsp;
column.3.valueformat=HTML
column.3.sharecol=true
column.4.valuefield=name
column.4.valueformat=HTML
column.4.sharecol=true
column.5.value=<br>
column.5.valueformat=HTML
column.5.sharecol=true
column.6.value=<b>Task Owner:</b>&nbsp;
column.6.valueformat=HTML
column.6.sharecol=true
column.7.valuefield=assignedTo:name
column.7.valueformat=HTML
column.7.sharecol=true
column.8.value=<br>
column.8.valueformat=HTML
column.8.sharecol=true
column.9.value=<b>Actual Completion Date:</b>&nbsp;
column.9.valueformat=HTML
column.9.sharecol=true
column.10.valuefield=actualCompletionDate
column.10.valueformat=HTML
column.11.displayname=Name of Reviewer
column.11.linkedname=Name of Reviewer
column.11.namekey=view.relatedcolumn
column.11.namekeyargkey.0=Name of Reviewer
column.11.namekeyargkey.1=name
column.11.querysort=DE:Name of Reviewer:name
column.11.valuefield=Name of Reviewer:name
column.11.valueformat=customReferenceObjectAsString
column.12.displayname=AAR 1
column.12.description=In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.12.value=<b>AAR 1 Score:</b>&nbsp;
column.12.valueformat=HTML
column.12.sharecol=true
column.13.valuefield=AAR 1 - In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.13.valueformat=customDataLabelsAsString
column.13.sharecol=true
column.14.value=<br>
column.14.valueformat=HTML
column.14.sharecol=true
column.15.value=<br><b>AAR 1 User Comment:</b>&nbsp;
column.15.valueformat=HTML
column.15.sharecol=true
column.16.valuefield=AAR 1 User Comment
column.16.valueformat=customDataLabelsAsString
column.17.linkedname=direct
column.17.namekey=AAR 1 Reviewer Comment
column.17.querysort=DE:AAR 1 Reviewer Comment
column.17.valuefield=AAR 1 Reviewer Comment
column.17.valueformat=customDataLabelsAsString
column.18.linkedname=direct
column.18.displayname=AAR 1 Needs Attn
column.18.querysort=DE:AAR 1 Needs Attention
column.18.valuefield=AAR 1 Needs Attention
column.18.valueformat=customDataLabelsAsString
column.19.linkedname=direct
column.19.displayname=AAR 1 Needs Attn Notes
column.19.querysort=DE:AAR 1 Needs Attention Notes
column.19.valuefield=AAR 1 Needs Attention Notes
column.19.valueformat=customDataLabelsAsString
column.20.displayname=AAR 2
column.20.description=Do You Believe This Work Will Make an Impact?
column.20.value=<b>AAR 2 Score:</b>&nbsp;
column.20.valueformat=HTML
column.20.sharecol=true
column.21.valuefield=AAR 2 - Do You Believe This Work Will Make an Impact?
column.21.valueformat=customDataLabelsAsString
column.21.sharecol=true
column.22.value=<br>
column.22.valueformat=HTML
column.22.sharecol=true
column.23.value=<br><b>AAR 2 User Comment:</b>&nbsp;
column.23.valueformat=HTML
column.23.sharecol=true
column.24.valuefield=AAR 2 User Comment
column.24.valueformat=customDataLabelsAsString
column.25.linkedname=direct
column.25.namekey=AAR 2 Reviewer Comment
column.25.querysort=DE:AAR 2 Reviewer Comment
column.25.valuefield=AAR 2 Reviewer Comment
column.25.valueformat=customDataLabelsAsString
column.26.linkedname=direct
column.26.displayname=AAR 2 Needs Attn
column.26.querysort=DE:AAR 2 Needs Attention
column.26.valuefield=AAR 2 Needs Attention
column.26.valueformat=customDataLabelsAsString
column.27.linkedname=direct
column.27.displayname=AAR 2 Needs Attn Notes
column.27.querysort=DE:AAR 2 Needs Attention Notes
column.27.valuefield=AAR 2 Needs Attention Notes
column.27.valueformat=customDataLabelsAsString
column.28.displayname=AAR 3
column.28.description=Are you proud of the work you did on this?
column.28.value=<b>AAR 3 Score:</b>&nbsp;
column.28.valueformat=HTML
column.28.sharecol=true
column.29.valuefield=AAR 3 - Are you proud of the work you did on this?
column.29.valueformat=customDataLabelsAsString
column.29.sharecol=true
column.30.value=<br>
column.30.valueformat=HTML
column.30.sharecol=true
column.31.value=<br><b>AAR 3 User Comment:</b>&nbsp;
column.31.valueformat=HTML
column.31.sharecol=true
column.32.valuefield=AAR 3 User Comment
column.32.valueformat=customDataLabelsAsString
column.33.linkedname=direct
column.33.namekey=AAR 3 Reviewer Comment
column.33.querysort=DE:AAR 3 Reviewer Comment
column.33.valuefield=AAR 3 Reviewer Comment
column.33.valueformat=customDataLabelsAsString
column.34.linkedname=direct
column.34.displayname=AAR 3 Needs Attn
column.34.querysort=DE:AAR 3 Needs Attention
column.34.valuefield=AAR 3 Needs Attention
column.34.valueformat=customDataLabelsAsString
column.35.linkedname=direct
column.35.displayname=AAR 3 Needs Attn Notes
column.35.querysort=DE:AAR 3 Needs Attention Notes
column.35.valuefield=AAR 3 Needs Attention Notes
column.35.valueformat=customDataLabelsAsString
column.36.displayname=Done
column.36.valuefield=Review Complete
column.36.valueformat=customDataLabelsAsString
```
