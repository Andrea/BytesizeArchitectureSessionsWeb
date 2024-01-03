---
layout: casa
title: En Español
author: Emilio Carrión
---

Muchas gracias a [Emilio Carrión](https://www.linkedin.com/in/emcarrio/) por traducir este contenido y hacerlo accesible a más gente. 
---

Las *Bytesize Architecture Sessions* son un formato de taller que ayuda a los equipos a comprender los sistemas en los que trabajan. Cada sesión se centra en una pequeña porción de un sistema. Tras algunas sesiones, tu equipo será más homogéneo en la comprensión de sus sistemas, desarrollará un vocabulario consistente y, en última instancia, construirá herramientas para diseñar el futuro juntos.

Una sesión dura entre 45 y 90 minutos, y consta de cuatro partes bien definidas: Objetivo de la sesión, *Alone Together*, Consenso y Resumen. Puedes modelar tus sistemas utilizando distintas herramientas. Sugiero empezar con Diagramas C4.

## ¿Preferirías ver un video?

Un video en inglés sobre por que existe este formato de taller y como puede ayudar a tu equipo 
<iframe title="vimeo-player" src="https://player.vimeo.com/video/842232215?h=129cccdf22" width="450" height="300" frameborder="0"    allowfullscreen></iframe> 

Otro video en inglés, tiene más tiempo para preguntas y respuestas al final de la presentación. 
<iframe width="450" height="300"  src="https://www.youtube.com/embed/uJ0f8fLU2Vw" title="YouTube video player" frameborder="0" allowfullscreen></iframe>

## ¿Por qué usar las *Bytesize Architecture Sessions*?

Considera usar las *Bytesize Architecture Sessions* si experimentas alguna de las siguientes dificultades comunes:

- Conocimiento de la base de código. La planificación de grandes cambios requiere un conocimiento sólido de los sistemas actuales. Los equipos pueden acabar con silos de conocimiento y no ver el panorama general
- Deuda técnica. El sistema ha crecido y no se ha atacado la complejidad accidental. Entender cómo resolver la deuda sin dejar de sacar funcionalidades requiere cierta planificación.
- Equipos en evolución. Es difícil mantener la cohesión de conocimientos en un equipo que ha cambiado con el tiempo.
- Todo lo anterior, probablemente agravado por problemas del proceso.

Estas son algunas de las mejoras que observé al realizar las sesiones con diferentes equipos. 
Los equipos

- Piensan en sus sistemas
- Desarrollan habilidades de modelización de sistemas
- Aprenden a modelar sistemas **juntos**, lo que mejora la dinámica de equipo
- A medida que se celebran más sesiones, tienen una comprensión cada vez más **homogénea** del sistema
- Perciben el valor de tener un modelo mental compartido
- Disponen de mejores herramientas para modelar posibles soluciones
- Aprenden a escuchar activamente

Las *Bytesize Sessions* son especialmente valiosas para los nuevos miembros del equipo o para aquellos con menos experiencia. Esto es especialmente cierto en equipos que no hacen *pair programming* o tienen silos profundos. Las Sesiones "abren el 'mundo'" Es difícil exagerar lo importante que es tener un modelo mental preciso y compartido. Los estudios demuestran que los modelos mentales son especialmente importantes a la hora de tomar decisiones difíciles y con limitaciones de tiempo (Besnard et al. #).

## ¿Quién organiza las *Bytesize Architecture Sessions*?

Cualquiera puede proponer una *Bytesize Sessions*. Las sesiones deben sentirse como propias del equipo.

Aunque no es obligatorio que haya un anfitrión, puede ser útil, sobre todo al principio. El papel del anfitrión es ser un facilitador, alguien que mantenga el ritmo de la sesión y centre el debate en el objetivo. El anfitrión puede ser cualquiera, no necesariamente alguien que dirija el equipo. El anfitrión debe cambiar de vez en cuando.

## Guía para organizar las primeras sesiones

![Overview](http://bytesizearchitecturesessions.com/images/bytesize-overview.png)

### Antes de la sesión, prepara a la gente
Uno de los principales objetivos de las *Bytesize Sessions* es que el equipo tenga un conocimiento homogéneo del sistema con el que trabaja. Las personas adecuadas para asistir son todas aquellas que tienen un alto nivel de influencia en ese sistema.

Empieza con un equipo. Invita a los que saben lo que hay que hacer, a los que construyen el sistema y a los que mejor entienden los requisitos de las partes interesadas. Si no estás seguro, empieza por las personas en *Stand Up*. Si hay más de diez personas en la lista de invitados, plantéate dividir la reunión en grupos más pequeños.

La herramienta de modelización recomendada para empezar es C4. Si el equipo no tiene experiencia con ella, entrénalo primero. Durante una *Bytesize Session*, los asistentes deben centrarse en el modelado, no en la herramienta de modelado elegida.

### Llevando a cabo una *Bytesize Architecture Session*
La clave de una buena sesión es asegurarse de que todo el mundo sabe lo que tiene que hacer. Al principio de la sesión, explica el formato general y, a continuación, profundiza en los detalles de cada sección.

#### Objetivo
Esta sección de la reunión debería durar unos cinco minutos y consiste en establecer un *Objetivo* para esta sesión en particular. Una buena primera sesión consiste en modelar el sistema en el que trabaja activamente el equipo *tal y como es en este momento*. Ten en cuenta que los asistentes dispondrán de pocos minutos para modelarlo. Si el sistema que se intenta modelar es demasiado grande, elige una subsección en la que centrarse.

Es bueno tener una sugerencia de qué modelar antes de empezar una sesión. Sin embargo, el objetivo final debe ser fruto del acuerdo del equipo.

Antes de pasar a la siguiente sección, comprueba que todos los asistentes entienden el objetivo.

#### *Alone Together*
Esta sección debería durar diez minutos o menos.

Para la primera parte de esta sección, programa un temporizador de tres a cinco minutos. Durante este tiempo todos trabajan individualmente y en silencio en la misma tarea de modelado. Una vez transcurrido el tiempo, cada uno explica su diagrama al resto del grupo.

Este modus operandi puede resultar atípico, pero he aquí algunas razones por las que resulta útil:

- El tiempo en silencio permite a las personas trabajar y pensar individualmente, sin las voces de los demás. Refuerza su concentración en el aspecto del sistema en el que se centra la sesión.
- Mayor compromiso con el tema durante el resto de la sesión.
- Ayuda a los participantes a autoevaluar la comprensión que tienen del sistema, destacando las áreas en las que pueden centrarse para aprender más.
- Entender qué piensan de los sistemas otras personas del equipo

![Image of participants with their individual models](/images/alone-together.png)

#### Consenso
La parte más larga de la sesión, que dura entre veinte y treinta minutos.

El **consenso** consiste en reunirse para crear un diagrama a partir de cero con los conocimientos combinados del equipo.

Es normal que las cosas se pongan un poco agitadas. Para lograr el objetivo, nombra a un escriba que puede rotar en cada reunión. El escriba dibujará el diagrama desde cero con la ayuda de todos.

El anfitrión desempeña un papel clave durante este tiempo si la conversación empieza a desviarse del objetivo de la sesión.

#### Resumen
Los últimos minutos de la reunión.

Se hace una retrospectiva del taller. Esta parte de la sesión consiste en revisar lo que se ha conseguido y lo que hay que hacer a continuación. Pon un cronómetro durante un minuto y pide a los asistentes que escriban en notas adhesivas lo que han aprendido y cualquier otro comentario.

Tarea extra opcional: pide a un voluntario que haga una copia en limpio del diagrama y que traiga a la próxima sesión las preguntas que queden pendientes.

#### ¡Repítelo!
La repetición es una forma estupenda de aprender, lo ideal es hacer otra sesión dentro de una semana o dos. No debe ser tan a menudo como para abrumar a la gente y debe ser lo suficientemente a menudo como para mantener la familiaridad con las cosas discutidas.

Las *Bytesize Sessions* pueden utilizarse para el aprendizaje continuo. También es posible establecer objetivos a largo plazo, por ejemplo, las *Bytesize Architecture Sessions* pueden utilizarse para crear una arquitectura objetivo o para facilitar la comunicación entre equipos en un trabajo complicado.


## Preguntas Frecuentes
### Cuáles son algunos síntomas de que se necesitan algunas *Bytesize Sessions*

- Está claro que las personas del equipo tienen un modelo mental incorrecto del sistema o que el modelo mental que tienen es incongruente con otras personas del equipo
- Cuando hay que tomar decisiones de diseño sólo habla una persona. Nadie más "sabe lo suficiente" para contribuir, ni siquiera con preguntas.
- Cuando hay que tomar decisiones de diseño, la discusión se eterniza y no se toma ninguna decisión (esto puede reflejarse como un cambio de decisión o que nadie "recuerda lo que decidimos al final")
- El equipo ha cambiado mucho o está formado en su mayoría por gente nueva

### Cómo se originó este formato
Empecé con las *Bytesize Architecture Sessions* alrededor de 2017. En el corazón de las sesiones está el tiempo *Alone Together*. Un breve espacio de tiempo en el que todos los participantes de la sesión trabajan por separado y en silencio en la misma tarea de modelado.

Después de muchas sesiones, la gente me pidió que escribiera sobre ello. Pensé que no era necesario porque es muy sencillo. Luego, me di cuenta de lo a menudo que utilizo y recomiendo la Técnica Pomodoro, con la ventaja añadida de que coordina a un equipo de personas.

## Más información pronto

Cualquier pregunta o comentario por favor contáctame a través de mastodon: @roundcrisis@types.pl