# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [29/10/2026] |
| Versión | [Versión de trabajo] |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como persona usuaria registrada, quiero buscar recetas por ingredientes o texto y excluir ingredientes, para encontrar recetas que se adapten a mis necesidades y consultar sus detalles.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

La épica resume los requisitos del documento sin entrar en detalles técnicos ni en reglas específicas de funcionamiento. Así, expresa el objetivo general de la funcionalidad de búsqueda y permite desarrollar posteriormente historias de usuario más concretas.

## US-01

**Título:** búsqueda de receta mediante una palabra o frase

como usuario quiero poder realizar la busqueda mediante una plabra o frase

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado un usuario que esta buscando recetas mediante una palabra o frase cuando el nombre contenga al menos una palabra o frase entonces el sistema muestra las recetas que tengan ficha palabra o frase
- **CA-02.** Dado un usuario que introduce una palabra o frase que coincide parcialmente con el nombre de una receta, cuando realiza la búsqueda, entonces el sistema muestra las recetas que contienen dicha coincidencia parcial.
- **CA-03.** Dado un usuario que introduce una palabra o frase con mayúsculas o minúsculas diferentes a las utilizadas en el nombre de la receta, cuando realiza la búsqueda, entonces el sistema devuelve las mismas coincidencias independientemente del uso de mayúsculas o minúsculas.
## US-02

**Título:** búsqueda por ingrediente incluido

como usuario quiero tener la capacidad para poder buscar recetas en base al ingrediente incluido en cada producto

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que el usuario que quiere tener la capacidad para poder buscar en base al ingrediente o ingredientes incluidos en cada producto cuando un ingrediente se repite en varias recetas entonces el sistema incluira todas las recetas con dichos ingredientes.
- **CA-02.** Dado que el usuario que quiere tener la capacidad para poder buscar en base al ingrediente o ingredientes incluidos en cada producto cuando un ingrediente no esta en ninguna receta entonces el sistema le comunicara que ese ingrediente no aparece en ninguna receta.
- **CA-03.** Dado que el usuario que quiere tener la capacidad para poder buscar en base al ingrediente o ingredientes incluidos en cada producto cuando un ingrediente este agotado entonces el sistema le comunicara que las recetas con dicho ingrediente estaran modificadas

## US-03

**Título:** excluir ingredientes

como usuario me gustaría poder buscar recetas por  excluir ingredientes .

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que el usuario le gustaria poder buscar recetas en base al ingrediente excluido cuando este ingrediente este seleccionado para excluir entonces el sistema solo mostrará recetas sin ese ingrediente.
- **CA-02.** Dado que el usuario ha seleccionado un ingrediente para excluirlo, cuando confirme la selección, entonces el sistema mostrará dicho ingrediente en la lista de ingredientes excluidos.
- **CA-03.** Dado que el usuario ha excluido ingredientes que están presentes en todas las recetas disponibles, cuando realice la búsqueda, entonces el sistema informará de que no se han encontrado recetas que cumplan los criterios de búsqueda.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | [Sí] | [Sí/No/Pendiente] | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | [Sí] | [Sí/No/Pendiente] | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | [Sí] | [Sí/No/Pendiente] | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | [Sí] | [Sí/No/Pendiente] | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | [Sí] | [Sí/No/Pendiente] | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | [Sí] | [Sí/No/Pendiente] | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
