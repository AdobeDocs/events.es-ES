---
title: Pregunte al experto - Medición de velocidad
description: Aprenda a medir y rastrear la velocidad mediante [!DNL Workfront] informes. Este taller se grabó el 14 de agosto de 2019.
activity: use
doc-type: feature video
team: Technical Marketing
jira: KT-9912
last-substantial-update: 2023-08-15T00:00:00Z
exl-id: 83053de2-e386-4243-a9c8-a2ad9d51790f
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '3958'
ht-degree: 1%

---

# Pregunte al experto - Medición de velocidad

Aprenda a medir y rastrear la velocidad mediante [!DNL Workfront] informes. Este taller se grabó el 14 de agosto de 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341057/?quality=12)

## Campos personalizados utilizados en la presentación

Ahorre tiempo copiando y pegando los cálculos siguientes.

>[!NOTE]
>
>La sintaxis para los cálculos de campos personalizados ha cambiado desde que se realizó la presentación en 2019, aunque los conceptos y otras instrucciones que se proporcionan en la presentación siguen siendo precisos.
>**Los cálculos que se incluyen a continuación se han actualizado para reflejar las reglas de sintaxis más recientes.**

**Fecha de primera confirmación**

Formato: Fecha

Cálculo:

```
IF(ISBLANK({DE:First Commit Date}),{defaultBaseline}.{plannedCompletionDate},{DE:First Commit Date})
```

**Primera duración**

Formato: Texto

Cálculo:

```
IF(ISBLANK({DE:First Duration}),{defaultBaseline}.{durationMinutes},{DE:First Duration})
```

**Proporción de trabajo a compromiso**

Formato:Número

Cálculo:

```
ROUND(DIV({actualDurationMinutes},{DE:First Duration}),1)
```

**Estado de relación trabajo-compromiso**

Formato:Texto

Cálculo:

```
IF({DE:Work-to-Commit Ratio}>2,"Terrible",IF({DE:Work-to-Commit Ratio}>1.6,"Poor",IF({DE:Work-to-Commit Ratio}>1.2,"Not Bad","Excellent")))
```

**Velocidad ajustada**

Formato:Número

Cálculo:

```
ROUND(DIV({actualDurationMinutes},{durationMinutes}),1)
```

**Estado de velocidad ajustado**

Formato:Texto

Cálculo:

```
IF({DE:Adjusted Velocity}>2,"Terrible",IF({DE:Adjusted Velocity}>1.6,"Poor",IF({DE:Adjusted Velocity}>1.2,"Not Bad","Excellent")))
```

## Preguntas y respuestas

**Pregunta**

Hola, gracias por organizar este seminario web. Tengo una pregunta sobre Field en Workfront. En nuestro sistema, hemos creado un campo personalizado llamado &quot;Estado&quot; que es una combinación de Estado y Condición. Este campo Estado contiene un montón de estatuas en miles de proyectos, lo que es muy importante para nuestro extracto de datos Tableau. Sin embargo, ahora queremos eliminar este campo y utilizar el campo Condición, el campo nativo. ¿Tiene alguna idea de cómo puedo voltear este campo sin perder datos? Todo lo que puedo pensar en hacerlo sin perder datos ahora es cambiarlos manualmente de un proyecto a otro.

**Respuesta**

En una situación como esta, puede utilizar el filtrado y la edición masiva para semiautomatizar la tarea de rellenar el campo Condición en función del campo personalizado de Estado.

A continuación se describen los pasos que debe seguir:

1. Determine qué valores de estado desea asignar a los valores de condición. Por ejemplo, supongamos que tiene un valor de estado de &quot;Late&quot; y &quot;Very Late&quot; que ambos asignan a un valor de condición de &quot;In Trouble&quot;
1. Cree un informe de proyecto que muestre todos los proyectos con un valor de estado de &quot;Retrasado&quot; y &quot;Muy atrasado&quot;.
1. Ejecute el informe. Asegúrese de que muestra todos los proyectos (consulte las opciones en la parte inferior derecha del informe)
1. Haga clic en la casilla de verificación situada en la parte superior izquierda del informe, en la barra con encabezados de columna. Se seleccionarán todos los proyectos del informe
1. Haga clic en el botón Editar situado encima de la lista de informes
1. Establezca el Tipo de condición en Manual
1. Establezca el campo Condición en Con problemas
1. Haga clic en Guardar cambios


**Pregunta**

¿Cómo se define Excelente, No malo, etc.?

**Respuesta**

Esto fue solo un ejemplo, pero así es como lo configuré. Primero calculé dos índices:

Velocidad ajustada

La fórmula para esto es Duración real/Duración planificada (que se almacena en el campo Duración de un proyecto). Dado que la duración planificada del proyecto puede cambiar cada vez que se replanifica el proyecto, la duración planificada representa la replanificación final.

Proporción de trabajo a compromiso

Esta fórmula es como Velocidad ajustada excepto que, en lugar de utilizar el valor Duración planificada de la replanificación final, queremos utilizar la Duración planificada que se prometió por primera vez al cliente. Suponemos que la línea de base original contiene esta información (y planeamos pedir a nuestros jefes de proyecto que planifiquen sus proyectos de esta manera para poder capturar datos precisos). Capturamos este valor de duración a partir de la línea de base original y lo llamamos Primera duración.

Al dividir la duración real entre la duración planificada o la primera duración, obtenemos un número que nos indica hasta dónde hemos llegado para llegar al objetivo. Si la Duración planificada o la Primera duración son iguales a la Duración real, el índice será igual a 1. Si la duración real es mayor, la respuesta será mayor que 1. Cuanto mayor sea el número peor lo hicimos en el cumplimiento de nuestra fecha.

Por lo tanto, dado todo lo que he decidido asignar estados tanto para la velocidad ajustada como para la relación trabajo-compromiso de la siguiente manera:

* 1,1 o menos yo llamé Excelente.
* De 1,2 a 1,5 llamé No está mal.
* De 1,6 a 1,9 llamé Pobre.
* 2 o más Yo llamé Terrible.

**Pregunta**

¿Qué debe hacer el trabajador para seguir la cantidad de tiempo que se tarda en hacer los proyectos?

**Respuesta**

No estamos rastreando las horas reales invertidas trabajando en los proyectos aquí, solo estamos rastreando y comparando la duración. Pero si está realizando un seguimiento de las horas y desea utilizar las horas reales sobre las planificadas para calcular la velocidad, puede realizar este mismo tipo de informe comparando las horas planificadas con las reales. También desea capturar las horas planificadas de la línea de base original.

**Pregunta**

¿Puede proporcionar los filtros utilizados para Velocity?

**Respuesta**

He utilizado dos reglas de filtro para los informes de Velocity:

* Categorías > ID > Igual >> Datos del proyecto WPI (este es el formulario personalizado que contenía todos los campos calculados). (Solo deseo ver los proyectos que estén utilizando este formulario personalizado)
* Proyecto > Estado > Igual > Completado (solo deseo ver los proyectos completados porque tienen un valor de Duración real que representa el tiempo que se ha tardado en realizar todo. Los proyectos actuales no proporcionarían una duración real precisa para calcular la velocidad)

También agregué otros filtros para mantener mi informe lo suficientemente pequeño como para administrarlo para el seminario web, pero en su entorno de producción probablemente desee ver todos los proyectos con el formulario personalizado WPI en un período de tiempo determinado. Es posible que desee filtrar la fecha real de finalización del proyecto para ese elemento.

**Pregunta**

Si copia un proyecto, ¿lleva las mismas líneas de base al nuevo proyecto?

**Respuesta**

No, las líneas de base no se incluyen en el proyecto copiado

**Pregunta**

Para un proceso de aprobación de tareas, ¿puede mostrarme cómo crear un informe que proporcione una pista de auditoría por tarea en un proyecto con una marca de fecha y hora para cada aprobador?

**Respuesta**

Crear un informe de tareas. En la pestaña Columnas (Ver), haga clic en Agregar columna. En el cuadro &quot;Mostrar en esta columna:&quot; escriba &quot;approv&quot;. Esto le mostrará los distintos campos de aprobación disponibles para informar. Le sugeriría que agregue una columna para todo al principio (excepto para los ID), para que pueda ver qué información se muestra.

A continuación, vaya a la pestaña Filtros y agregue una regla de filtro para:

La Tarea >> Es La Aprobación >> Igual >> Verdadero. Esto solo mostrará las tareas que tengan una aprobación adjunta.

Añada filtros adicionales según sea necesario.

**Pregunta**

Me gustaría crear un informe de prueba. Una lista de proyectos que muestre cuántas pruebas tienen y cuántas versiones de esa prueba existen.

**Respuesta**

Crear un informe de documento.

La vista predeterminada muestra el número de versión. Querrá dejar eso allí, pero puede cambiar cualquier otra columna.

Agrupar el informe por nombre de proyecto.

Filtrar el informe por versión actual: el ID de prueba no está en blanco.

Esto le proporcionará una lista de todas las pruebas de cada proyecto. Tendrá una fila para cada prueba y mostrará el número de versión (que será el mismo que el número total de versiones).

**Pregunta**

¿Se puede utilizar Velocity en el nivel de tarea? ¿En lugar de nivel de proyecto?

**Respuesta**

Sí, pero deberá copiar el formulario personalizado del proyecto y crear un formulario personalizado de tarea a partir de él. A continuación, deberá editar el cálculo en el campo Primera fecha de confirmación y cambiar la referencia a &quot;Línea de base predeterminada&quot; por &quot;Tarea de línea de base predeterminada&quot;. Haga lo mismo para Primera duración. Después, puede adjuntar el formulario personalizado a cualquier tarea que desee medir. Deberá crear informes de tareas en lugar de informes de proyectos para estos. Sin embargo, tendrá que asegurarse de que la línea de base del proyecto original está establecida como línea de base predeterminada. Todos los datos de la tarea se mantienen en la misma línea de base con los datos del proyecto.

**Pregunta**

¿El propietario del proyecto tiene que establecer manualmente la primera fecha de confirmación? ¿O podría extraer de los campos existentes?

**Respuesta**

La fecha de primera confirmación se captura de la línea base predeterminada. Siempre que la línea de base predeterminada sea la línea de base original, se mostrará la fecha planificada de finalización del proyecto en el momento en que se estableció por primera vez en Estado actual.

**Pregunta**

¿Siguen siendo correctos los campos calculados en los formularios personalizados y deben actualizarse periódicamente? ¿O sucederá automáticamente de la noche a la mañana (o en algún otro déclencheur) ahora?

**Respuesta**

Los campos calculados se vuelven a calcular:

* Cuando un usuario edita el objeto
* Edición masiva con expresiones personalizadas de Recalcular activadas
* Modificaciones en el formulario con la opción seleccionada &quot;Actualizar cálculos anteriores&quot;

**Pregunta**

Si la velocidad está considerando la duración, ¿debe basarse el porcentaje completado en la preferencia de proyecto en la duración?

**Respuesta**

No, la opción Preferencias del proyecto sólo hace referencia a cómo se calcula el porcentaje completado. El valor de duración en sí no se ve afectado por esta configuración.

**Pregunta**

¿Cuál es la diferencia entre la primera y la duración del plan?

**Respuesta**

Primera duración es el número de días que prometió originalmente al cliente que tomaría el proyecto. Obtenemos este número de la línea de base original que se registró cuando el proyecto cambió de Planificación a Actual.

Duración planificada es el número de días desde el inicio del proyecto hasta la fecha planificada de finalización. Inicialmente estas dos duraciones son iguales, pero si el proyecto se replanificó alguna vez y la fecha planificada de finalización cambió, también lo hizo la duración planificada.

El valor de los informes de Velocity se debe a que hemos podido ver cuánto ha cambiado la duración planificada con respecto a la primera duración. Podemos ver esto tan atrás como cuando empezamos a registrar líneas de base a medida que los proyectos cambiaban de Planificación a Actual.

**Pregunta**

¿Se pueden definir los trabajadores por color para que sean iguales en todos los informes?

**Respuesta**

Si agrupa por Asignado a >> Nombre en un informe de tareas, puede asignar un color a determinados trabajadores en la pestaña Gráfico. Simplemente, elija la opción Colores personalizados junto al cuadro Asignado a >> Nombre en la ficha Gráfico y agregue un color para cada trabajador.

**Pregunta**

Estoy intentando determinar si es posible crear un panel con un área que busque un formulario personalizado de nivel de tarea para ver si está presente y es secundario si ciertos campos no están en blanco. ¿Es esto posible?

**Respuesta**

Vamos a ver si entiendo tu pregunta. Supongamos que tengo un formulario personalizado de tareas llamado Formulario Tammy con un campo llamado Campo Tammy.

Desea un informe de tareas que muestre todas las tareas que tienen un formulario Tammy adjunto y en las que el campo Tammy tiene algún valor.

Sí, puedes hacer eso. Solo necesita un filtro en el informe de tareas con dos reglas de filtro:

Categorías >> Formulario de Tammy igual a ID

Tarea > El Campo Tammy No Está En Blanco

**Pregunta**

¿Existe alguna forma de crear un informe para buscar un documento con nombre específico en la biblioteca de documentos? Parte del tablero que queremos medir si existen ciertos documentos.

**Respuesta**

Sí. Debe crear un informe de documento. Parece que desea proporcionar un nombre de documento específico cada vez que ejecuta el informe. Si ese es el caso, recomendaría ir a Opciones de informe y seleccionar Indicadores de informe. Añada una solicitud para Documento > Nombre.

**Pregunta**

¿Puede elegir un color / valor hexadecimal que no aparece en la pestaña del gráfico, pero que es un nuevo color que es un nuevo valor hexadecimal, por ejemplo, un nuevo color de mis colores de marca para permitirme personalizar los informes?

**Respuesta**

Sí, puede escribir cualquier código de RGB que haya podido encontrar. Este es un código estándar que indica la cantidad de rojo, verde y azul que contiene el color. Workfront aceptará cualquier valor hexadecimal de 000000 a FFFFFF, por lo que si conoce el código de su color de marca puede utilizarlo.

**Pregunta**

¿Podría volver a exponer la definición de los informes en el tablero (proporcionar una declaración de lo que mide cada informe)?

**Respuesta**

Gráfico de estado de velocidad ajustado

> Esto muestra lo bien que lo hicimos al completar los proyectos a tiempo al comparar la duración real del proyecto con la duración planificada. La duración planificada se ha ajustado porque el proyecto se ha replanificado durante su ciclo de vida.

Gráfico de estado de relación trabajo-compromiso

> Esto muestra lo bien que lo hicimos al completar los proyectos a tiempo al comparar la duración real del proyecto con la primera duración. Siendo la Primera Duración el tiempo original que le prometimos al cliente que el proyecto tardaría en completarse. La primera duración se calculó a partir del valor Duración del proyecto cuando se cambió por primera vez de Planificación a Estado actual. Duración registrada en la línea de base original.

Informe de lista de estado de velocidad

> Este informe contiene todos los campos personalizados calculados y las fechas significativas para los mismos proyectos en los gráficos. Su propósito es permitirnos comprobar nuestros cálculos y obtener información más detallada si lo desea.

**Pregunta**

¿Cómo se agregaron los nuevos datos al eje x?

**Respuesta**

Cuando se agrupa por cualquier elemento de un informe, se puede crear un gráfico. A continuación, puede establecer el eje X o Y en la pestaña Gráfico.

**Pregunta**

¿Puede ver la diferencia entre la primera duración y la duración real?

**Respuesta**

Primera duración es el número de días que prometió originalmente al cliente que tomaría el proyecto. Obtenemos este número de la línea de base original que se registró cuando el proyecto cambió de Planificación a Actual.

La duración real es el número de días desde el comienzo del proyecto hasta la fecha real de finalización.

**Pregunta**

¿Cómo se integra el factor de línea de base del proyecto en este informe?

**Respuesta**

La línea de base original del proyecto contiene la fecha planificada de finalización y la duración planificada que existía cuando el proyecto se cambió por primera vez al estado Actual. Si el proceso tuviera que planificar el proyecto antes de establecerlo en Actual, entonces esto representaría la fecha en la que se comprometió a completar el proyecto antes del.

**Pregunta**

¿Hay alguna forma de aplicar de forma masiva el nuevo formulario a proyectos antiguos?

**Respuesta**

Sí, puede seleccionar varios proyectos de una lista. Al hacerlo, aparecerá la opción &quot;Editar&quot; en la parte superior izquierda de la lista. Al hacer clic en Editar cuando se seleccionan varios objetos, se encuentra en lo que llamamos &quot;edición masiva&quot;. Puede agregar un formulario personalizado a varios proyectos de esta manera.

Un método abreviado para agregar formularios personalizados a un gran número de proyectos es crear un informe que filtre para incluir solo los proyectos que desee. A continuación, en lugar de seleccionar proyectos individualmente, simplemente haga clic en la casilla de verificación situada encima de la primera casilla de la lista y seleccionará la lista completa.

**Pregunta**

¿Es posible quitar las entradas duplicadas de la agrupación en un informe de asignación, pero no entre agrupaciones?

**Respuesta**

La mejor manera de ver las agrupaciones en los informes de listas es esta:

En primer lugar, se controla qué elementos aparecen en la lista mediante la ficha Filtro. No habrá entradas duplicadas. El filtro se aplica a cada objeto. Si pasa por el filtro, aparecerá una vez en la lista; si no lo hace, no aparecerá en absoluto.

La siguiente agrupación se aplica a la lista filtrada. Una agrupación identifica una cosa acerca de los objetos de la lista, como el nombre del portafolio en el que se encuentra (no se puede agrupar en una lista de cosas, solo en una). A continuación, todos los objetos con el mismo valor aparecerán en esa agrupación, como todos los proyectos del mismo portafolio. Los proyectos que no tengan seleccionado un portafolio aparecerán en la agrupación denominada &quot;Sin valor&quot;.

Como resultado, no hay forma de que los objetos puedan aparecer en más de una agrupación. El filtro controla totalmente si un objeto aparece en la lista (y si la persona que ejecuta el informe tiene derechos para verlo).

**Pregunta**

¿Recomendaría algún otro informe para rastrear Velocity? Solo una recomendación de alto nivel es genial porque sé que no hay suficiente tiempo para ir a través de los detalles.

**Respuesta**

Al igual que con cualquier informe, lo primero que debe hacer es decidir lo que desea saber. El siguiente paso es acceder a esa información, lo que en algunos casos significa que debe iniciar el seguimiento.

Una razón por la que decidí comparar la Duración real con dos tipos de Duración planificada fue porque pensé que me proporcionaba perspectivas interesantes sobre la velocidad. Los datos también ya estaban disponibles, así que no tuve que empezar a rastrearlos. Con algunos cálculos podría extraer los datos en un formulario del que podría informar.

Pero también puede decidir realizar un seguimiento de otra información acerca de tareas o proyectos para crear informes.

Workfront no tiene ningún informe de velocidad integrado, por lo que le recomendaría a usted y a su equipo que piensen en lo que desea saber para determinar la velocidad y luego vean lo que necesitan rastrear.

**Pregunta**

¿Puede calcular algo en el nivel de COLUMNA? En lugar de llamar a un campo calculado desde un formulario personalizado

**Respuesta**

Habría sido posible utilizar una expresión de valor en modo de texto para realizar estos cálculos. Sin embargo, no podríamos haber hecho Primera duración o Primera fecha de compromiso, necesitábamos capturar a los que estaban en un lugar donde no cambiarían.

En cuanto al estado de la relación trabajo-compromiso y el estado de velocidad ajustado, estos debían ser campos personalizados para que pudiéramos utilizarlos en la pestaña Gráfico. La pestaña Gráfico no reconoce las agrupaciones en modo de texto, deben ser campos personalizados. Y como necesitábamos una relación trabajo-compromiso y una velocidad ajustada para calcular esos estados, también los necesitábamos para ser campos personalizados. Por lo tanto, en este caso, todos tenían que ser campos personalizados, pero siempre es bueno tener en cuenta ambas formas y elegir qué es lo que mejor funciona. Gracias por la pregunta.

**Pregunta**

Nuestros proyectos cambian a menudo debido a retrasos de clientes o cambios a lo largo de. Nuestro informe podría mostrar todo como &quot;terrible&quot;. ¿Qué es una recomendación para rastrear motivos de cambio? Se ha pensado en agregar un formulario personalizado al nivel de documento que informe del motivo del cambio (ya sea un cambio interno o de cliente), pero se ha preguntado cuál es la práctica recomendada.

**Respuesta**

La práctica recomendada es utilizar un menú desplegable para rastrearlo. Ponga tantas &quot;razones&quot; como pueda pensar para empezar, luego añada una opción &quot;otro&quot; para capturar una razón que no está en la lista. Si esa nueva razón se ve o se vuelve común, agréguela a la lista desplegable. Puede informar fácilmente sobre las cosas en una lista desplegable y puede agrupar en este campo (no puede agrupar en casillas de verificación o en una lista desplegable de selección múltiple).

Solo otro comentario sobre esto. Es posible que no desee incluir todos los proyectos en los informes de Velocity. Si estás arreglando errores o &quot;yendo a donde nadie ha ido antes&quot; probablemente no estás haciendo el mismo tipo de compromiso con una fecha de finalización que si estás construyendo una casa que has construido muchas veces antes.

Así que asegúrate de enfocar tu informe de velocidad en lugares donde pueda ayudarte a alcanzar tus metas.

**Pregunta**

Si establecí la línea de base predeterminada de un proyecto en &#39;Original&#39; y luego quito el proyecto de la línea de base actual y lo vuelvo a poner en la línea de base actual, ¿cambiará mi línea de base predeterminada?

**Respuesta**

Sí. Cada vez que cambie el estado a Actual obtendrá una nueva línea de base y será la nueva predeterminada. Sin embargo, todas las líneas de base anteriores seguirán existiendo y podrá establecer manualmente que la línea de base original vuelva a ser la línea de base predeterminada.

**Pregunta**

¿Existe alguna forma de configurar en un informe qué campos son editables? ¿Puedo establecer restricciones para determinados campos?

**Respuesta**

Puede restringir los derechos de visualización y edición de los campos de un formulario personalizado. Deberá incluir los campos en una sección y, en la configuración de la sección, puede elegir los derechos necesarios para que los usuarios puedan ver o editar los campos de la sección.

**Pregunta**

¿Puede crear un informe que busque un documento con nombre específico en la biblioteca de documentos?

**Respuesta**

Sí. Debe crear un informe de documento. Parece que desea proporcionar un nombre de documento específico cada vez que ejecuta el informe. Si ese es el caso, recomendaría ir a Opciones de informe y seleccionar Indicadores de informe. Añada una solicitud para Documento > Nombre.

**Pregunta**

En los informes, ¿por qué los valores están disponibles como columnas pero no como selecciones o grupos? Por ejemplo: Origen del problema.

**Respuesta**

La razón principal por la que una columna puede estar visible, pero no está disponible para la agrupación, es que podría contener una lista, como un campo personalizado de casillas de verificación o asignaciones de tareas. No se permite agrupar en una lista.

**Pregunta**

¿Cómo puedo separar en un informe (mediante qué campos) cuándo se produjo la entrada de horas y cuándo se realizaron realmente las horas?

**Respuesta**

El campo Fecha de entrada del objeto Hour hace referencia a la fecha en la que se trabajaron las horas. Esto hace que la fecha de entrada sea diferente a la de otros objetos, donde significa la fecha en la que se creó el objeto. Aunque no haya una fecha de creación para las horas, existe una &quot;Fecha de última actualización&quot; que es inicialmente la fecha de creación y, a continuación, cualquier fecha en la que se editó la hora.

**Pregunta**

Desde el punto de vista de los informes, ¿cómo podemos acceder a los datos de línea de base? Tengo un proyecto con varias líneas de base. Quiero ver cómo se planificaron las tareas individuales en cada línea de base. ¿Existe alguna forma de escribir un informe que muestre el plan del proyecto para cada línea de base?

**Respuesta**

En un informe se mostrarán los campos que desee ver para la línea de base que está establecida actualmente como predeterminada, por lo que puede cambiar la línea de base y actualizar el informe para ver los campos con la nueva línea de base.

Sin embargo, si desea ver información sobre las tareas gráficamente, puede hacerlo mediante la función de gráfico Gantt. Activa Gantt en una lista de tareas (usando el icono de Gantt en la esquina superior derecha junto a Guardar automáticamente), luego ve al icono de Configuración justo debajo y a la derecha y haz clic en él. Marque la casilla Línea Base y se mostrarán todas las líneas base. Puede seleccionarlos de uno en uno y ver los cambios en las tareas en la vista Gantt.

**Pregunta**

Cómo crear un informe para buscar los cambios en su estado durante un periodo definido, por ejemplo, el mes pasado.

**Respuesta**

La función Analytics de Workfront ofrece una forma sencilla de ver los datos históricos, incluidos los cambios de estado.

Sin embargo, también puede obtener información sobre el cambio de estado mediante un informe Nota. Puede filtrar para ver los cambios de estado en los proyectos si realiza el seguimiento del campo Estado del proyecto.

En primer lugar, vaya a Configuración>Interfaz>Actualizar fuentes y asegúrese de que el estado del proyecto es uno de los campos integrados de los que se realiza un seguimiento. Si no lo es, tiene que agregarlo.

Ahora cree un informe Nota y haga lo siguiente:

En la pestaña Columnas (Ver):

* Reemplace la columna &quot;Texto de la nota&quot; por &quot;Texto de auditoría&quot;. Esto mostrará información sobre qué estado ha cambiado de y a
* Deje las columnas &quot;Project: Name&quot; y &quot;Entry Date&quot;
* Haga clic en la columna &quot;Fecha de entrada&quot; y, a continuación, marque &quot;Ordenar por esta columna&quot; en el panel Configuración de columna. Si desea ver los cambios de estado más recientes en la parte superior, ordénelos en sentido descendente.

En la pestaña Groupings:

* Agrupar por proyecto: nombre

En la pestaña Filters, cree las siguientes reglas de filtro:

* Nota > Tipo de auditoría > Igual > Cambio de estado
* Añada reglas adicionales para filtrar por Fecha de entrada de nota. Es posible que prefiera dejar esto fuera de los Filtros y utilizar un mensaje de informe en su lugar
* Filtre por proyecto, portafolio u otros datos como desee.

**Pregunta**

¿Cómo planificador puede extraer informes para otros usuarios?

**Respuesta**

Un planificador puede crear informes y compartirlos con cualquier usuario, incluso con personas que no sean usuarios. Cuando visualice el informe, vaya a Acciones de informe>Compartir y, a continuación, haga clic en el icono de engranaje en la parte superior derecha del cuadro Acceso a informes. Elija la opción &quot;Convertir esto en público para los usuarios externos&quot;. JVM. Puede copiar el vínculo proporcionado y enviarlo a cualquier persona. Verán el informe en tiempo real en el explorador.
