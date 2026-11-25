# 6. Herramientas y gastos

Este documento asigna un papel a cada suscripción y recomienda qué mantener. Los precios y los planes verificados están en el [Anexo C](anexos/c_precios_y_planes.md).

## 6.1 Recomendación

| Suscripción | Costo actual | Papel en la fábrica | Recomendación |
| --- | --- | --- | --- |
| Claude Max | US$ 100 | Es el motor local. Lee las carpetas, ejecuta código y escribe en Notion, Drive y Gmail. | Se mantiene. |
| Google AI Pro | US$ 20 | Es el almacén. También ofrece un segundo modelo y cuadernos para consultar documentos. | Se mantiene. |
| Grok | US$ 30 | Es el trabajador en la nube. Tiene una computadora persistente con navegador propio. | Se mantiene. |
| ChatGPT Plus | US$ 20 | Su uso baja cada mes. Claude ya cubre el estudio y los textos de trabajo. | Pasa a la versión gratuita. |
| Notion | US$ 0 | Es el tablero de pedidos. | Sigue gratis. |

El gasto baja de US$ 170 a US$ 150 al mes. El ahorro es de US$ 240 al año.

## 6.2 Por qué se mantiene el agente en la nube

La primera versión de este análisis recomendaba cancelar Grok. Esa recomendación era un error, porque no conocía su uso real.

El agente en la nube cumple seis funciones.

| Función | ¿Claude la cubre? |
| --- | --- |
| Correr encargos con la PC apagada | Sí. Las tareas programadas en la nube corren con una hora de intervalo mínimo. |
| Vigilar temas con una frecuencia fija | En parte. Claude sirve para la web abierta, pero no lee X y consume el límite del plan. |
| Buscar en la web y entregar un reporte | Sí. |
| Entrar a un sitio que exige sesión y descargar archivos | No con la PC apagada. Con la PC encendida, Claude usa el navegador del usuario y se detiene en la pantalla de ingreso. |
| Trabajar en una máquina virtual persistente | En parte. La máquina de Claude en la nube nace vacía en cada corrida. |
| Ejecutar flujos de automatización | En parte. Existe una opción en la API, pero exige más montaje. |

La documentación de Claude no describe un equivalente a una computadora persistente que inicie sesión en sitios web. El detalle está en el [Anexo D](anexos/d_claude_sin_supervision.md).

## 6.3 Tres notas sobre Claude

1. **Créditos de API.** El plan Max incluye US$ 100 al mes en créditos de API. Los créditos caducan cada mes y se reclaman en la configuración de facturación. Hoy nadie los usa.
2. **Modelo por estación.** El plan incluye el modelo Fable solo hasta la mitad del límite semanal. Las estaciones rutinarias deben correr con un modelo menor.
3. **El plan Pro no alcanza.** El plan Pro cuesta US$ 20, da la quinta parte del uso y cobra el modelo Fable aparte.

## 6.4 Por qué no hace falta pagar Notion

El plan Business de Notion cuesta US$ 20 por usuario. Su ventaja son los agentes propios de Notion. Las tareas programadas de Claude cubren esa función y ya están pagadas. Falta comprobar en la práctica que esas tareas alcanzan a Notion.

El plan gratuito limita cada archivo a 5 MB. Ese límite no estorba, porque el tablero guarda enlaces y no guarda archivos.

## 6.5 Lo que no se pudo verificar

- Las páginas oficiales de Grok y de ChatGPT no mostraron precios. Se usaron los montos que informó el responsable.
- No se conoce cuánto del límite semanal de Claude se consume.
- No se probó la búsqueda web dentro de una tarea programada de Claude.
