---
layout: post
title:  Caso de estudio en una empresa de television britanica
date:   2024-01-03 10:53:25 
lang: es
author: Andrea Magnorsky
categories: case-study spanish 
---

Cuando trabajaba con una organización en la industria de televisión, tres equipos estuvieron involucrados en importantes mejoras en el flujo de trabajo de transmisión de video. Los tres equipos tuvieron que trabajar en conjunto debido a las dependencias entre su trabajo. 

![Dependencias de equipo](/images/team-dependencies.png)

El primer equipo tiene procesos que dependen del segundo equipo, y el segundo equipo inicia procesos en el tercer equipo. Y los equipos necesitaban mantenerse al tanto del progreso en los otros equipos. Por ejemplo, el primer equipo necesitaba saber cuándo se completaban los procesos en el tercer sistema.

Todos los involucrados conocían este nivel de dependencia mutua, y entendíamos que era probable que hubiéramos confiado en aspectos internos de los servicios en los que no deberíamos haberlo hecho, pero no sabíamos dónde estaban esas ineficiencias.

Organizamos Bytesize Architecture Sessions, los participantes eran dos programadores de cada equipo y un líder técnico que tenía conocimientos en el área en su totalidad. El objetivo principal era pensar en qué sería una arquitectura simple y buena. Además, teníamos un buen entendimiento compartido de los requisitos del producto, especialmente porque el proceso que estábamos explorando estaba bien establecido.

Durante la primera sesión se trató de modelar el sistema tal como estaba en ese momento. Utilizamos [Diagramas de contexto C4](https://c4model.com/#SystemContextDiagram) para dibujar lo que cada persona sabía sobre estos tres equipos trabajando juntos. Esta parte de una Bytesize Session, Alone Together, se realiza de forma individual donde los participantes trabajan por su cuenta. Se aprendió mucho durante este primer taller, por ejemplo, aprendimos detalles concretos sobre cómo funcionaba el proceso en cada uno de los equipos, en lugar de las suposiciones difusas que cada uno de nosotros hacía. También nos dimos cuenta de que el proceso que iniciaba todo se ejecutaba de formas ligeramente diferentes por dos equipos diferentes, lo que generó dos áreas principales de investigación: ¿Por qué estamos consumiendo la misma información de dos lugares diferentes? Y, ¿cuánto trabajo extra estamos haciendo que probablemente no necesitamos hacer?
Después de la sesión, capturamos algunas preguntas que necesitaban respuesta para la próxima sesión. Por ejemplo, necesitábamos detalles sobre una parte del API de uno de los servicios, y también teníamos algunas preguntas para las personas en equipos que no estaban representados en la reunión.

La siguiente sesión fue aproximadamente cuatro semanas después (hubiera sido mejor que sea dos semanas después). El objetivo de la sesión era modelar cómo debería lucir el sistema dada la problemática que teníamos que abordar. Mientras estábamos en la sección de _Consensus_ del taller, nos dimos cuenta de que algunos aspectos del flujo de trabajo, tal como era en ese momento, eran mucho más complicados de lo necesario, una ocurrencia común en las sesiones de bytesize. Por ejemplo, encontramos lógica duplicada que no nos estaba dando ninguna ventaja. También nos dimos cuenta de que podríamos mejorar una de las entradas del sistema, eliminando una deuda técnica bien conocida, pero olvidada.

Exploramos el problema con la lógica duplicada y nos dimos cuenta de que la cantidad de trabajo necesario para solucionarlo sería difícil de negociar, pero tomamos notas, con la esperanza de abordar este problema eventualmente. Luego procedimos a discutir los detalles de cómo debería lucir la interacción entre los tres sistemas en un mundo ideal.

Unos días después, uno de los equipos redactó un ADR para el contrato sobre lo que cambiaría y lo circuló a los otros dos equipos. Hubo algunos detalles que necesitaban ser aclarados y organizamos una videollamada improvisada para tratar el asunto. Treinta minutos después, todos los detalles estaban en su lugar.
En este punto, todos tenían todo el contexto necesario para resolver el problema. 

Estas sesiones de arquitectura Bytesize mejoraron las relaciones entre los equipos, por lo que estaban perfectamente preparados para abordar colaborativamente este desafío interno de la manera óptima.

En este ejemplo particular, todas las sesiones fueron remotas. Me gustaría enfatizar que he dirigido *Bytesize Architecture Sessions* tanto de forma remota como en persona, y los beneficios son grandes en ambos casos. Las sesiones también pueden funcionar en un formato híbrido. Básicamente, las dirijo como si todos estuvieran remotos para asegurarme de que la sesión incluya a todos.
