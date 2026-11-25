# 4. Archivo y búsqueda

Este capítulo describe cómo ordenar los archivos y cómo encontrarlos después. Es el primer trabajo de construcción.

## 4.1 El problema

Los archivos están repartidos en seis lugares y suman cerca de 344 000. El detalle está en el [diagnóstico](02_diagnostico.md). Ordenar y buscar a mano consume tiempo y produce copias.

## 4.2 Cuatro decisiones de diseño

1. **Tres zonas.** La zona Entrada reúne la bandeja y las descargas. La zona Vivo es la carpeta de trabajo de Drive. La zona Histórico reúne todo lo demás.
2. **Lo histórico se cataloga y no se mueve.** Mover 300 000 archivos viejos cuesta mucho y arriesga mucho. De esos archivos solo se necesita una cosa: encontrarlos. Un catálogo resuelve esa necesidad.
3. **Solo se ordena lo vivo.** Las reglas de nombre ya existen: `N_Tema` para las carpetas permanentes y `AAAAMMDD_Tema` para lo fechado.
4. **Se usa el método de la biblioteca.** El método tiene inventario, plan, aprobación y registro para deshacer. Nada se borra.

## 4.3 Mapa de procesos

| N.º | Proceso | Insumo | Método | Resultado |
| --- | --- | --- | --- | --- |
| 1 | Inventariar | Todas las ubicaciones del alcance | Un guion anota la ruta, el tamaño, la fecha y el tipo de cada archivo. | Un inventario único |
| 2 | Diagnosticar | El inventario | El guion cuenta por zona, tipo y año, y detecta copias idénticas. | Un informe de exploración |
| 3 | Definir la estructura | El informe | El responsable decide las carpetas y las reglas. Claude propone. | Un esquema de carpetas y nombres |
| 4 | Planificar | El inventario y el esquema | El sistema clasifica cada archivo vivo, primero con reglas y después con IA. | Un plan de movimientos para aprobar |
| 5 | Ejecutar | El plan aprobado | El guion mueve cada archivo, registra el movimiento y verifica los bytes. | Un almacén ordenado |
| 6 | Indexar | El almacén | El guion extrae el texto de los PDF y de los Word. | Una búsqueda por nombre y por contenido |
| 7 | Mantener | La bandeja y las descargas | La estación Entrada corre cada semana. | Una bandeja vacía |

Los procesos 1 y 2 solo leen. Ningún archivo cambia antes del proceso 5.

## 4.4 Tres niveles de búsqueda

| Nivel | Pregunta que responde | Herramienta |
| --- | --- | --- |
| Por nombre | ¿Dónde está el archivo? | El catálogo y las reglas de nombre |
| Por contenido | ¿Qué archivo menciona este término? | Un índice del texto extraído |
| Por significado | ¿Qué dice la norma sobre este tema? | La estación Consulta, con cita verificada |

Los dos primeros niveles funcionan con guiones y no consumen uso de IA.

## 4.5 Reglas de seguridad

- Ningún archivo se borra.
- Las copias idénticas pasan a una carpeta de revisión.
- El responsable aprueba el plan antes de cualquier movimiento.
- Cada movimiento queda en un registro que permite deshacerlo.
- El guion compara los bytes de origen y de destino.

## 4.6 Alcance propuesto

| Entra al inventario | Queda fuera |
| --- | --- |
| Drive: carpeta viva y carpeta histórica | Películas y música |
| Descargas, Escritorio y Documentos | Programas |
| Respaldos del disco D | La biblioteca ya ordenada |
| Respaldos de PC antiguas | Los repositorios de código |

El responsable debe confirmar este alcance. También debe decidir si entran los respaldos que pertenecen a otras personas.

## 4.7 Un arreglo pequeño pendiente

La guía de trabajo cita un libro con una ruta que ya no existe. Falta corregir esa ruta.
