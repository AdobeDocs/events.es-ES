---
title: Consulte al experto - Informes de modo de texto básico de sobrecarga mediante el Explorador de API
description: Obtenga información sobre el explorador de API, cómo utilizarlo y cómo mejorar sus informes aprovechando el modo de texto básico. Este seminario web se grabó el 22 de enero de 2020.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9918
exl-id: ea4716c9-2c61-4c44-9d2a-cbd4f07699d5
source-git-commit: ca06e5a8b1602a7bcfb83a43f529680a5a96bacf
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 2%

---

# Consulte al experto - Informes de modo de texto básico de sobrecarga mediante el Explorador de API

Obtenga información sobre el explorador de API, cómo utilizarlo y cómo mejorar sus informes aprovechando el modo de texto básico. Este seminario web se grabó el 22 de enero de 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341124/?quality=12)

## Recursos adicionales

![Gráfico que muestra ejemplos de reglas de código de modo de texto](assets/text-mode-chart.png)


**Columna final &quot;Todos los roles&quot;**

```
description="Primary =" indicates the user's primary job role
displayname=All Job Roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("Primary = ",{role}.{name}),{role}.{name})
valueformat=HTML
```

**Modo de texto para la columna &quot;Todos los equipos&quot;**

```
displayname=All Teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

**Modo de texto para la columna &quot;Todos los grupos&quot;**

```
displayname=All Groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

**Modo de texto para la columna &quot;Informes directos&quot;**

```
displayname=Direct Reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

## Preguntas y respuestas

**Pregunta**

¿Es posible utilizar cualquier colección en un informe utilizando el modo de texto?

**Respuesta**

Sí, puede utilizar cualquier objeto del área de colecciones. Va a querer explorar y ver a qué tiene acceso. No todo tendrá acceso al objeto de usuario y al objeto de rol como vimos con el objeto de roles de usuario en el explorador de API.

**Pregunta**

¿Puede comentar el &quot;uso condicional de diferentes colecciones en la misma columna (actualizaciones de proyectos frente a actualizaciones de tareas)&quot;?

**Respuesta**

Cuando se encuentra en el área de iteración y ve el campo de valor o la expresión de valor allí, está accediendo a uno de los elementos de la lista de la colección. Con el campo de valor podemos obtener el nombre de ese rol, por ejemplo, o cualquier cosa que esté en ese elemento de la lista. Si se encuentra en una tarea, un objeto de tarea puede hacer referencia al proyecto en el que se encuentra.

**Pregunta**

¿Puede discutir si la colección &quot;actualizaciones de tareas&quot; solo es posible en un informe de tareas?

**Respuesta**

Al crear un informe de problemas, puede ver la información de la tarea si el problema se notificó en relación con la tarea y también puede ver esa información desde la colección. Excepto en esas situaciones, deberá estar en un informe de tareas para ver los datos de recopilación de tareas.

**Pregunta**

¿Puede compartir el formato de texto ([!DNL CSS]) ejemplos?

**Respuesta**

Workfront no es compatible [!DNL CSS] en modo de texto.

**Pregunta**

¿Cuál es la mejor manera o la más rápida de localizar un nombre de campo personalizado para la creación de informes en modo de texto? He utilizado la opción de edición del HTML en el navegador OR añadiendo un campo en un informe y cambiando al modo de texto para agarrarlo PERO... curioso cómo otros realizan esto

**Respuesta**

Lo más rápido es seleccionar el campo en la interfaz de usuario, cambiar al modo Texto y copiar el nombre del campo. Esto garantiza que se escriba correctamente el campo.

**Pregunta**

¿Cómo se puede utilizar el modo de texto para identificar a los miembros de un equipo en un informe? Actualmente utilizamos asignaciones de equipos en flujos de trabajo de aprobación de tareas y nos gustaría enumerar los integrantes del equipo en la fase de aprobación actual en una columna similar a cómo funciona el campo Aprobadores y Estado.

**Respuesta**

Para hacer referencia a los integrantes del equipo asociados con la fase de aprobación actual, debe hacer referencia a una colección de una colección a la que se hace referencia, lo que actualmente no es posible mediante las funciones de modo de texto de Workfront. La columna que utiliza actualmente su organización y que muestra el equipo asociado con la aprobación es la mejor opción.

**Pregunta**

¿El campo y el nombre del objeto deben estar en mayúsculas o minúsculas correctamente (p. ej., rol vs rol)?

**Respuesta**

Cuando haga referencia a objetos en modo de texto, querrá escribirlos exactamente como se muestra en la columna derecha del Explorador de API. Por ejemplo, si desea hacer referencia a un nombre de proyecto a partir de un informe de tareas, el campo de valor tendría el siguiente aspecto:

```
valuefield=project:name
```

Sin embargo, en el caso de los problemas, se denominan &quot;opTasks&quot; en el Explorador de API. Por lo tanto, si ejecutara un informe de horas y deseara agregar una columna para el nombre del problema, el campo de valor tendría el siguiente aspecto:

```
valuefield=opTask:name
```

**Pregunta**

Estoy buscando generar un informe que muestre para cada proyecto las tareas activas actuales en las que se está trabajando. ¿Cómo puedo hacerlo mejor? Imagino que sería un informe de tareas que también tendría columnas de información del proyecto agregadas.

**Respuesta**

Eso es correcto. Para ello, sería mejor un informe de tareas. Debe definir &quot;Tareas activas&quot;. Si está utilizando predecesoras, entonces serían tareas que están Listas. Por lo tanto, puede filtrar por Listo = Verdadero. Esto traería todas las tareas que estén Listas para iniciarse. A continuación, le recomendaría que agrupe por nombre de proyecto, de esta forma todas las tareas se agrupan y puede ver de un vistazo qué tareas pertenecen a qué proyecto.

**Pregunta**

¿Hay alguna forma de crear informes que calculen datos (por ejemplo, % de proyectos que cumplan determinados criterios)?

**Respuesta**

La mejor manera de crear un informe para presentar o calcular datos (% por ejemplo) sería aplicar agrupaciones al informe y, a continuación, aplicar un gráfico. Si desea agregar un gráfico circular al informe, tiene la opción de que los sectores estén en valores o porcentajes.

**Pregunta**

¿Puede utilizar el modo de texto para identificar a los miembros de un equipo que están asignados a la fase de aprobación de la tarea actual de forma similar a las columnas Aprobadores y Estado?

**Respuesta**

Debe agregar una columna de colección en modo de texto al informe de tareas con lo siguiente:

```
displayname=Current Approval Stage Approvers 
listdelimiter=<p> 
listmethod=nested(currentApprovalStep.stepApprovers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

**Pregunta**

¿Puede filtrar dónde Todos los grupos contienen un grupo en particular?

**Respuesta**

Si desea filtrar los elementos del informe, debe hacerlo en la pestaña filtrar del informe. Por lo tanto, si desea ver solo los usuarios en los que uno de sus grupos sea Contabilidad, agregue una regla de filtro que diga:

```
Other Groups>ID>Equal>Accounting
```

**Pregunta**

¿Existe alguna forma de crear un informe que determine la duración real de una combinación de tareas?

**Respuesta**

Debe filtrar el informe para incluir únicamente la combinación de tareas que desee. A continuación, debe colocar una columna Duración real en la vista y resumirla por Suma en Configuración de columna; por último, debe agrupar el informe de alguna manera. Al ejecutar el informe, la barra de agrupación mostrará el total de las duraciones reales contenidas en las filas que se están agrupando.

**Pregunta**

¿Existe alguna forma de restar las tareas que caen dentro de un elemento principal para determinar la duración del resto de las tareas dentro de un elemento principal?

**Respuesta**

La duración de una tarea principal se calcula restando la fecha de inicio de la primera tarea inicial desde la fecha de finalización de la última tarea final debajo de esa tarea principal. En un informe solo se conoce si se debe mostrar o no cada tarea individual que se esté considerando. El motor de informes no tiene forma de conservar la información de una tarea y utilizarla cuando se mira otra tarea. Por lo tanto, la única manera de lograr lo que se está pidiendo es quitar una tarea para que no esté debajo de un elemento principal determinado mientras se encuentra en la lista de tareas de proyecto y observar cómo se vuelve a calcular la duración de la tarea principal.

**Pregunta**

Para las agrupaciones condicionales, una forma personalizada (por ejemplo, &quot;Estados occidentales&quot;, &quot;Estados centrales&quot; o &quot;Estados orientales&quot;) para descodificar los grupos individuales es una técnica común que funciona bien en ese aspecto, ¿cuándo se recomienda utilizar agrupaciones calculadas o parámetros calculados?

**Respuesta**

Las agrupaciones calculadas (también conocidas como expresiones de valor en una agrupación) son una forma cómoda de obtener un resultado que se mostrará en la barra de agrupación. Esto también se puede hacer mediante un campo personalizado calculado. Hay pros y contras para cada enfoque, que son:

* Las expresiones de valor se calculan cada vez que se actualiza la página del explorador. Esto puede ser mejor que los campos personalizados calculados que se vuelven a calcular cada vez que se edita el objeto al que están adjuntos, o cuando los campos calculados se vuelven a calcular en una edición masiva, o cuando se edita el formulario personalizado y se selecciona la opción &quot;Actualizar cálculos anteriores&quot;.
* Sin embargo, las expresiones de valor no se pueden utilizar en gráficos, formatos condicionales ni filtros. Deberá utilizar campos personalizados calculados para estos.

**Pregunta**

¿No hay forma de cambiar el nombre para mostrar de la agrupación de &quot;Sin valor&quot; a cualquier otra cosa que elijamos para llamarla con fines de creación de informes? en otras palabras, ¿SIEMPRE será &quot;Sin valor&quot;?

**Respuesta**

Hay una manera de reemplazar &quot;Sin valor&quot; con algo diferente. Supongamos que tiene un informe de proyecto agrupado por Nombre de Portfolio. Todos los proyectos que no están asignados a un portafolio terminarán en una agrupación con el título:

```
Portfolio: Name: No Value
```

Para cambiar esto, edite la agrupación en modo de texto y reemplace esta línea:

```
group.0.valuefield=portfolio:name
```

con esta línea:

```
group.0.valueexpression=IF(ISBLANK({portfolio}.{name}),"Not in any Portfolio",{portfolio}.{name})
```

La agrupación tendrá ahora este título:

```
Portfolio: Name: Not in any Portfolio
```

**Pregunta**

¿Hay un parámetro para rastrear asignaciones incompletas, es decir:

1. Tareas con una sola asignación a la que no se le asignó un individuo o
1. Tareas con varias asignaciones que tienen al menos una persona sin asignar para las funciones solicitadas

**Respuesta**

Esto se puede lograr utilizando un informe de asignación y filtrando para

```
Assigned To ID > Is Blank and Role ID > Is Not Blank
```

Esto extraerá todas las tareas o problemas que se hayan asignado a una función, pero no necesariamente a un usuario específico. Deberá agregar las columnas Nombre de tarea y Nombre de problema para ver a qué objeto pertenece la asignación y, si se agrupa por Nombre de proyecto, ayudará a mantenerla organizada.

**Pregunta**

Chuck, lo olvido, pero ¿recuerdas la propiedad en modo texto que luego se renderiza como información sobre herramientas, al pasar el ratón por encima?

**Respuesta**

description= permite mostrar información del objeto al pasar el ratón por encima del encabezado de la columna.

**Pregunta**

¿Puedo informar sobre un campo de casilla de verificación que permita varias selecciones, pero que solo extraiga la primera selección al informe?

**Respuesta**

Sí. Las opciones seleccionadas en el campo de casilla de verificación están todas en una cadena con cada selección separada por una coma. Utilizará la expresión SEARCH para buscar la posición de la primera coma en el campo Casilla de verificación y, a continuación, utilice ese índice con la expresión LEFT para mostrar esos caracteres desde el principio de la lista. Este es el código:

```
valueexpression=IF(SEARCH(",",{DE:Checkbox Field},0)>0,LEFT({DE:Checkbox Field},SEARCH(",",{DE:Checkbox Field},0)),{DE:Checkbox Field})
```

Si utiliza una coma en un nombre de selección en el campo de casilla de verificación, solo se mostrará la parte de esa selección hasta la primera coma.
