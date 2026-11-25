# werk

Fábrica personal de trabajo con IA: un sistema para archivar, buscar y producir documentos con calidad constante.

**Estado:** análisis y diseño, al 25 de noviembre de 2026. Todavía no se construyó nada.

## Resumen en una página

**La pregunta.** ¿Se puede construir una «fábrica» que cubra todo el trabajo, desde ordenar y buscar información hasta producir productos? ¿Se puede gastar menos en suscripciones?

**La respuesta.** Sí se puede, y cerca de la mitad ya existe. No hace falta pagar otra herramienta. Faltan tres piezas: un índice único, una entrada ordenada y un control de calidad.

**Las fuentes.** El análisis parte de dos textos. El artículo «A New Shape for Work», de Notion, dice qué construir. El libro *Scaling People*, de Claire Hughes Johnson, dice cómo operarlo.

**El diseño.** La fábrica tiene seis estaciones: Vigilancia, Entrada, Consulta, Producción, Entrega y Mejora. Un agente en la nube vigila y hace encargos. Claude archiva, busca con cita y produce. La persona responsable decide y firma.

**El orden.** Primero se ordena el archivo, porque todo lo demás depende de encontrar las fuentes. Después se construye la primera línea de producción: la carpeta de reunión.

**El gasto.** El gasto mensual baja de US$ 170 a US$ 150. Se mantienen Claude, Google y Grok. ChatGPT pasa a la versión gratuita y Notion sigue gratis.

## Documentos

| N.º | Documento | Contenido |
| --- | --- | --- |
| 1 | [Fuentes](docs/01_fuentes.md) | Qué dicen el artículo y el libro, y qué se toma de cada uno. |
| 2 | [Diagnóstico](docs/02_diagnostico.md) | Qué existe hoy y qué falta, con mediciones. |
| 3 | [Diseño de la fábrica](docs/03_diseno.md) | Las estaciones, las reglas de gobierno y la primera línea. |
| 4 | [Archivo y búsqueda](docs/04_archivo_y_busqueda.md) | El plan para ordenar y catalogar los archivos. |
| 5 | [Inventario de skills](docs/05_inventario_skills.md) | Cómo clasificar lo que la fábrica sabe hacer. |
| 6 | [Herramientas y gastos](docs/06_herramientas_y_gastos.md) | El papel de cada suscripción y la recomendación. |

Los anexos guardan la evidencia:

- [Anexo A](docs/anexos/a_articulo_notion.md): el artículo de Notion, sección por sección.
- [Anexo B](docs/anexos/b_scaling_people.md): las ideas del libro que se usan aquí.
- [Anexo C](docs/anexos/c_precios_y_planes.md): los precios y planes verificados.
- [Anexo D](docs/anexos/d_claude_sin_supervision.md): lo que Claude puede hacer con la PC apagada.

## Decisiones pendientes

1. **Alcance del inventario.** Falta confirmar qué ubicaciones entran y cuáles quedan fuera.
2. **Inventario.** Falta autorizar la corrida del proceso 1, que solo lee los archivos.
3. **Respaldos de otras personas.** Falta decidir si entran al catálogo.
4. **Reportes del agente en la nube.** Falta fijar la carpeta donde deben caer.
5. **Primera carpeta de reunión.** Falta elegir la reunión real para la prueba.
6. **Inventario de skills.** Falta clasificar las 46 entradas y completar sus tres datos.

## Siguiente paso

El siguiente paso es el proceso 1 del [capítulo de archivo](docs/04_archivo_y_busqueda.md): el inventario de todas las ubicaciones.

## Glosario

- **Agente:** un asistente de IA que ejecuta pasos, y no solo conversa.
- **Sistema de contexto:** el lugar donde vive lo que la IA necesita saber para trabajar.
- **Fábrica:** un sistema de agentes dedicado a una tarea específica, compartido y vigilado.
- **Estación:** una etapa de la fábrica, con un insumo, un método y un resultado.
- **Línea de producción:** la secuencia de pasos que produce un tipo de documento.
- **Skill:** un paquete de instrucciones que Claude carga cuando aparece una tarea conocida.
- **Conector:** el enlace que permite a un asistente leer y escribir en otra aplicación.
- **Corrida en sombra:** una prueba en la que la fábrica produce un borrador en paralelo al trabajo manual.
- **Catálogo:** una tabla con una fila por archivo, que permite buscar sin mover nada.
