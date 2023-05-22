---
title: 'Pregunte al experto: comprensión de la combinación y la capacidad'
description: Aprenda a medir la combinación y la capacidad dentro de su empresa. Este seminario web se grabó el 2 de octubre de 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9913
source-git-commit: edd0bdb28a9b3d065a64a95af6a216b747577c77
workflow-type: tm+mt
source-wordcount: '2224'
ht-degree: 1%

---

# Pregunte al experto: comprensión de la combinación y la capacidad

Aprenda a medir la combinación y la capacidad dentro de su empresa. Este seminario web se grabó el 2 de octubre de 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341119/?quality=12)

## Preguntas y respuestas

**Pregunta**

¿Cómo se coloca %s en un gráfico de columnas?

**Respuesta**

Los valores % enumerados en el informe de mezcla estaban ahí porque en la pestaña de gráfico elegimos &quot;Agrupar columnas&quot; y &quot;Apiladas al 100 %&quot;. Si elegimos &quot;Apilado&quot;, se mostrarían los totales de horas planificados y no el porcentaje.

**Pregunta**

Si la carga de trabajo de su departamento u organización es una combinación de proyectos/tareas y problemas/solicitudes, ¿cómo recomienda obtener una revisión de alto nivel (en un informe de Workfront) de un WPI?

**Respuesta**

Los proyectos, las tareas y los problemas deben tener sus propios informes con sus propios formularios personalizados. Sin embargo, cada uno puede utilizar el mismo campo de tipo de trabajo. Puede que desee mostrar los tres informes en un tablero.

**Pregunta**

¿Es necesario editar las tareas de forma masiva para hacerlas operativas o estratégicas?

**Respuesta**

La técnica que sugerimos es crear un informe que le permita obtener una lista de las tareas que están operativas. Una vez que sepa que puede seleccionar todas las tareas a la vez, edítelas por lotes, adjunte el formulario personalizado con Tipo de trabajo y establezca el tipo de trabajo en Operativo para todas las tareas a la vez. Siga el mismo procedimiento de adquisición para recopilar una lista de tareas estratégicas, editarlas en lote y agregar el formulario personalizado, etc.

En el seminario web se mencionan algunas ideas para mensajes personalizados que podrían ayudarle a obtener una lista, como comprobar ciertas palabras en el nombre de la tarea, el propietario del proyecto, el portafolio o los usuarios asignados. Estas son solo ideas. Debe diseñar un informe que funcione mejor en su situación.

**Pregunta**

Si tengo 4 categorías en mi mezcla, ¿puedo crear una meta para cada una y luego informar sobre el delta entre previsión vs. plan vs. real? (4 categorías Campaña, Unidad de negocio, Web y Producto). Tenemos las categorías en el nivel de proyecto en formularios/campos personalizados. El objetivo sería crear una previsión trimestral (presupuesto/previsión) y luego rastrear las horas planificadas hasta esa previsión y, en última instancia, las reales.

**Respuesta**

Si tiene todas las categorías en un campo personalizado (llamémoslo Tipo de trabajo por ahora), solo tiene que crear un grupo de informes de proyecto en Horas planificadas primero y Tipo de trabajo segundo. Filtre el informe de proyecto para mostrar los proyectos de Planning en los intervalos de fechas deseados. Utilice un gráfico con columnas agrupadas o barras apiladas al 100% si desea ver porcentajes. Podría ser su informe de pronóstico.

Puede copiar el informe y editarlo para crear un informe basado en Proyectos actuales, que siga mostrando la combinación basada en las Horas planificadas.

Puede volver a copiar el informe, cambiarlo a grupo por horas reales en lugar de horas planificadas y mostrar solo los proyectos completados dentro de los intervalos de fechas deseados. Esto mostraría la combinación porcentual en función de las horas reales.

**Pregunta**

¿Funcionará esto si tiene varios ID de categoría en un proyecto o tarea?

**Respuesta**

Sí, si tiene varios ID, deben separarse con una pestaña, de esta manera:

```
EXISTS:1:$$EXISTSMOD=NOTEXISTS
EXISTS:1:$$OBJCODE=OBJCAT
EXISTS:1:categoryID=5d76d82600e7926bb51eeb1e0886810e 5d54288d01034619f2eb2c74f6472f18
EXISTS:1:objID=FIELD:ID
```

La mejor manera de separarlos con un carácter de tabulación es crear primero la lista de categorías en el generador. Coloque varios nombres de formulario personalizados y, cuando cambie al modo de texto, los verá como ID separados por tabulaciones.

Los ID múltiples se tratan como OR, por lo que si alguno de ellos está adjunto a la tarea, no aparecerá en el informe.

**Pregunta**

¿Se muestran las indicaciones del informe en &#39;ANDed&#39; o en &#39;ORed&#39;?

**Respuesta**

Los mensajes personalizados individuales son &quot;ANDed&quot;. Por lo tanto, si especifica Pam como propietario del proyecto y Bill como asignado a la tarea, solo verá las tareas asignadas a Bill que estén en proyectos en los que Pam sea el propietario del proyecto.

**Pregunta**

¿Por qué solo puede ordenar por determinadas columnas? es decir, no se puede ordenar por asignaciones.

**Respuesta**

&quot;Asignaciones&quot; es una lista y no puede ordenarla o agruparla en una lista de elementos. Solo puede ordenar o agrupar por un elemento individual.

Para ilustrar el punto, imagine una lista de asignaciones como esta en una tarea:

```
Jane
Bill
Dan
```

Y una lista de asignaciones como esta en otra tarea:

```
Bill
Jane
Helen
```

¿Qué tarea debe aparecer primero en una ordenación? Podría decir &quot;ordenar por el nombre en la lista&quot;, pero esto no es necesariamente útil, ya que no puede controlar el orden. Workfront evita el problema al no permitirle ordenar por listas.

¿Qué sucede con la agrupación por lista? Si pudiéramos agrupar por una lista de nombres encontraríamos todas las tareas asignadas a Jane, Bill, Dan agrupadas y todas las tareas asignadas a Jane, Dan, Bill (la misma lista, pero en un orden diferente) en una agrupación diferente. De nuevo, Workfront evita el problema al no permitir la agrupación por listas.

**Pregunta**

¿Se utilizan las horas planificadas para tareas estratégicas y las horas reales para operaciones?

**Respuesta**

No. En nuestro ejemplo utilizamos las horas planificadas para mostrar el nivel de esfuerzo planificado tanto para tareas estratégicas como operativas. Esto nos permite compararlos fácilmente, ya sea en el pasado, presente o futuro. También puede utilizar horas reales para comparar tareas estratégicas y operativas, pero solo para tareas del pasado, ya que las horas reales son las horas que las personas han informado como el tiempo que realmente han invertido trabajando en las tareas.

**Pregunta**

En el planificador de recursos, ¿cómo se contabilizan las tareas que se planificaron en el pasado, pero que no se completaron? Las horas planificadas no parecen moverse hacia adelante y, por lo tanto, no se muestran en semanas futuras como tareas/horas que necesitan recursos.

**Respuesta**

No hay desplazamiento &quot;automático&quot; hacia adelante de trabajo no completado. Cuando esto ocurra, deberá volver a planificar el proyecto. Es posible que los recursos que asignó originalmente a una tarea determinada no estén disponibles en el nuevo periodo de tiempo, por lo que el administrador del proyecto debe ver esto y decidir la mejor manera de volver a planificar. Esto puede implicar la participación de las partes interesadas y la obtención de aprobaciones para los cambios en el plan.

**Pregunta**

En lugar de introducir 2 horas al día para comprobar el correo electrónico y las pausas, ¿recomienda ajustar su valor de FTE?

**Respuesta**

Sí, si establece el valor de FTE en 0,75, se mostrará al usuario como disponible 6 horas al día en el Planificador de recursos. Esta será su disponibilidad todos los días. Si desea mostrarlos como no disponibles para diferentes períodos según la fecha, como no disponible el último día de cada trimestre, la forma de hacerlo es mediante un proyecto de costes generales.

Algunas personas prefieren los proyectos generales porque pueden construirlos ellos mismos y cambiarlos cuando quieran, mientras que es posible que no tengan derechos para editar su propio ETC.

**Pregunta**

¿Los datos del tablero de capacidad del equipo están disponibles para cualquier persona con la que comparta el informe, independientemente de los permisos que tengan sobre el trabajo?

**Respuesta**

Si un usuario no tiene permiso para ver el objeto, no será visible dentro del informe/panel. Sin embargo, si desea que todos vean los mismos resultados, puede ir a Acciones de informe > Editar > Configuración de informe e introducir su nombre en el campo, &quot;Ejecutar este informe con los derechos de acceso de&quot;. Esto permitirá a los usuarios que se comparten en este informe ver los resultados exactos que ve. No les otorgará acceso adicional al resultado en sí, por lo que algunos resultados pueden o no ser seleccionables.

**Pregunta**

¿Cómo se puede crear un informe que muestre todo el personal asignado a un proyecto en general (no en el nivel de tarea)?

**Respuesta**

Puede crear una columna dentro de un informe de proyecto que muestre todos los usuarios enumerados como parte de la ficha Asignación de personal (Equipo del proyecto). Debe utilizar el siguiente modo de texto:

```
displayname=Project Team
listdelimiter=<p>
listmethod=nested(projectUsers).lists
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

**Pregunta**

Me gustaría tener un informe/panel que incorpore el funcionamiento de mi equipo. En particular los siguientes escenarios: - Proyectos de mi propiedad / Proyectos creados para mí / Tareas asignadas a otros / Tareas asignadas a mí

**Respuesta**

Proyectos de mi propiedad

Hay un informe integrado llamado &quot;Proyectos actuales&quot; que le mostrará todos los proyectos actuales. Puede editar este proyecto y añadir una regla de filtro: Proyecto > ID del propietario > Igual a > $$USER.IDTuando guardar y cambiar el nombre del informe a &quot;Proyectos de mi propiedad&quot;.

Proyectos creados para mí

Hay un informe integrado llamado &quot;Mis proyectos&quot; que le mostrará todos los proyectos actuales en los que esté en el equipo del proyecto (lo que significa que es el propietario, patrocinador o asignado a una tarea). No estoy seguro de si esto es lo que está pidiendo, pero no hay otra manera de saber si alguien creó un proyecto para usted que no sea hacerle propietario del proyecto, patrocinarlo o asignarle a una tarea.

Tareas asignadas a otros usuarios

Cree un informe de tareas con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar a modo de texto. Agregue este código a lo que ya esté allí:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Esto le mostrará todas las tareas en las que el usuario que ha iniciado sesión ha asignado al menos a uno de los usuarios asignados actualmente. Si varias personas han asignado a las personas, solo el nombre de la primera persona que asignó a alguien aparecerá como &quot;Solicitado por&quot; en la página de aterrizaje de la tarea. Si desea ver todas las personas asignadas y que asignaron cada una, puede agregar una columna a la vista, cambiar al modo de texto y reemplazar lo que haya con esto:

```
displayname=All Assignees and Requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

Tareas asignadas a mí

Hay un informe integrado llamado &quot;Mis tareas&quot; que le mostrará todas las tareas incompletas en Proyectos actuales en los que usted es el propietario de la tarea. Le sugeriría que cambie el filtro para mostrarle todas las tareas en las que es uno de los muchos usuarios asignados potencialmente, no solo el propietario de la tarea. Para ello, elimine la regla de filtro

```
Task > Assigned To ID > Equal > $$USER.ID 
```

y sustituyéndolo por

```
Assignment Users > ID > Equal > $$USER.ID
```

**Pregunta**

¿Hay alguna manera de personalizar las etiquetas en los gráficos? He descubierto que cuando creo un gráfico para reflejar los estados del proyecto- el nombre del grupo de inicio termina siendo incluido en la etiqueta.

**Respuesta**

Las etiquetas de los gráficos utilizan el nombre de campo de aquello en lo que está agrupando. Por lo tanto, la única manera de cambiar las etiquetas es utilizar un campo personalizado calculado con el nombre que desee. En la sección de cálculo del campo, escriba el nombre del campo nativo por el que desea agrupar.

**Pregunta**

¿Cómo codifica con color las barras de informes de las asignaciones de equipo de Chuck, por favor? Es decir, ámbar para detrás, rojo para tarde y verde para a tiempo? ¿También puede cambiar el orden para que sea más lógico, es decir, rojo/ámbar/verde o al revés?

**Respuesta**

Para cambiar los colores utilizados en el informe para las opciones de Progress Status, edite el informe y haga clic en la pestaña Chart. Busque la lista desplegable &quot;Colores personalizados >&quot;. Aparecerá junto al cuadro &quot;Eje izquierdo (Y)&quot; o al cuadro &quot;Agrupar datos por&quot;, dependiendo de si decide agrupar o no columnas o barras. En esa lista desplegable puede seleccionar colores. Si haces clic en los números en la parte inferior derecha de las opciones de color, podrás seleccionar tu color de una paleta más grande.

Lamentablemente, no puede cambiar el orden de estos elementos.

**Pregunta**

¿Puede crear un gráfico donde señale al Recuento de proyectos en los que un trabajador tiene asignada una tarea?

**Respuesta**

Sí, así es como:

* Creación de un informe de proyecto
* Si el usuario en cuestión es el usuario que ha iniciado sesión, el filtro debe incluir esta línea:

```
   Project Users > ID > Equal >$$USER.ID 
```

* Si no es así, coloque el nombre de usuario en lugar de [!DNL $$USER.ID]. Se mostrarán todos los proyectos en los que esta persona tenga asignada una tarea, sea el propietario o el patrocinador. Si solo desea ver los proyectos en los que se les han asignado tareas, debe agregar estas dos reglas de filtro adicionales:

```
   Project > Owner ID > Not Equal > $$USERID
   Project > Sponsor ID > Not Equal > $$USERID
```

* Cree al menos una agrupación para poder crear un gráfico. Agrupar en cualquier cosa, como compañía. A continuación, haga clic en la pestaña Chart y seleccione un gráfico. &quot;Recuento de registros&quot; será el valor predeterminado para un eje. Este será el número de proyectos en los que el usuario tenga una asignación.

Cuando se asigna a un usuario una asignación en un proyecto (asignada a un propietario de tarea o proyecto o patrocinador de proyecto), esa persona se agrega al equipo del proyecto y se puede ver en la pestaña Asignación de personal, en la subpestaña Personas. Si se quita a un usuario de ser el propietario del proyecto, patrocinador o de tener asignaciones de tareas, su nombre sigue estando en el equipo del proyecto. Si desea eliminarla, debe eliminarla manualmente. Tenga en cuenta que esto podría afectar a la precisión de los resultados del informe. Para eliminar a alguien del equipo del proyecto, vaya a Asignación de personal > Personas, seleccione la persona o personas y, a continuación, haga clic en el botón Eliminar que aparece encima de la lista.

**Pregunta**

¿Cómo puede cambiar el orden descendente de una columna en el modo de texto (en una agrupación)?

**Respuesta**

Puede elegir ordenar la mayoría de las columnas en la pestaña Columnas (Ver) al crear un informe. Esto ordenará todo el informe de lista si no tiene agrupaciones. Si tiene agrupaciones, se ordenarán según esa opción dentro de cada agrupación.

**Pregunta**

¿Cómo puedo crear una columna que identifique a los integrantes del equipo asignados a una fase de aprobación?

**Respuesta**

Si está ejecutando un informe de tarea o problema/solicitud, existe una columna disponible dentro del Report Builder llamada &quot;Aprobadores y estado&quot; que extraerá esta información.
