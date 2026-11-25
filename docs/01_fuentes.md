# 1. Fuentes

Este documento resume los dos textos que originan el proyecto. También dice qué se acepta y qué se descarta de cada uno.

## 1.1 El artículo: «A New Shape for Work»

Notion publicó este texto en 2026 como una guía de campo de unas diez mil palabras. El detalle por sección está en el [Anexo A](anexos/a_articulo_notion.md).

**Qué sostiene.** El artículo defiende dos ideas.

1. La IA rinde poco sin un *sistema de contexto*. Un sistema de contexto es un lugar único donde vive lo que la IA necesita saber.
2. El trabajo repetido debe pasar a *fábricas*. Una fábrica es un sistema de agentes dedicado a una tarea específica, compartido y vigilado.

**Qué se acepta.**

- El contexto va antes que los agentes. Sin contexto, cada conversación empieza de cero.
- La frase central es correcta: «alquila la inteligencia, sé dueño del contexto».
- Una fábrica debe ser específica, compartida y vigilada.
- La fábrica más simple es una lista de pedidos con una columna de estado.
- Antes de confiar en una fábrica, conviene probarla con corridas en sombra.

**Qué se descarta.**

- Las cifras del artículo no tienen fuente. Ejemplos: «mil veces más capaz» y «cinco minutos para montarla».
- El argumento económico supone equipos de 25 a 100 personas. En esos equipos, muchas personas se reparten el costo fijo.
- El artículo presenta a Notion como el único almacén posible. El mismo texto admite que los agentes pueden correr en Claude o en código propio.

**Qué cambia para una sola persona.** El retorno no viene del número de usuarios. El retorno viene de la repetición en el tiempo. Por eso solo merece una línea de producción lo que se repite. «Compartido» significa aquí tres cosas: entre equipos (PC y laptop), entre asistentes y con uno mismo en el futuro.

## 1.2 El libro: *Scaling People*

Claire Hughes Johnson fue directora de operaciones de Stripe. Su libro trata de dirigir personas en una empresa que crece. Las notas de lectura están en el [Anexo B](anexos/b_scaling_people.md).

El libro aporta lo que al artículo le falta: cómo se gobierna el sistema. De él se toman cuatro ideas.

1. **La casa.** Una organización necesita documentos fundacionales, un sistema operativo y una cadencia. Los documentos fundacionales dicen para qué existe. El sistema operativo fija las normas compartidas. La cadencia fija el ritmo de revisión.
2. **Pocos procesos obligatorios.** Cada proceso común tiene un costo de coordinación. Conviene imponer muy pocos.
3. **Delegar según impacto y reversibilidad.** Casi todo se delega, salvo lo que tiene alto impacto y no tiene vuelta atrás. Cada trabajo tiene un responsable directo.
4. **Higiene de procesos.** Hay que desconfiar de los procesos defensivos y de los procesos que envejecen. Un proceso nuevo se prueba con plazo y con criterio de evaluación.

## 1.3 Cómo encajan las dos fuentes

El artículo dice qué construir. El libro dice cómo operarlo.

| Concepto del artículo | Concepto del libro | Pieza de la fábrica |
| --- | --- | --- |
| Sistema de contexto | Documentos fundacionales y comunicación interna | Almacén, catálogo y reglas |
| Ontología con pocas bases de datos | Carta de equipo: misión, clientes, métricas, riesgos e interfaces | Ficha de cada estación |
| Fábrica específica, compartida y vigilada | Propiedad y mecanismos de rendición de cuentas | Estaciones con responsable y registro |
| Jefe de fábrica | Responsable directo (DRI) | Responsable de cada línea |
| Corridas en sombra y evaluaciones | Experimentos con plazo y criterio | Estación Mejora |
| Disparadores programados | Cadencia operativa | Tareas programadas y revisión semanal |

## 1.4 Un límite que se respeta

El objetivo del responsable no es solo obtener resultados. También quiere entender el trabajo y poder explicarlo. Por eso la fábrica no reemplaza el aprendizaje. Cada estación conserva su mapa de procesos, con insumo, método y resultado.
