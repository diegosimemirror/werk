# werk: contexto para continuar

Este archivo orienta a Claude cuando trabaja en este repositorio. El resumen del proyecto está en `README.md`.

## Qué es

`werk` es el proyecto de una fábrica personal de trabajo con IA. Cubre el archivo, la búsqueda y la producción de documentos. Todo el desarrollo del proyecto se guarda aquí.

## Estado al 25 de noviembre de 2026

- El análisis y el diseño están escritos en `docs/`.
- No se construyó ninguna estación.
- Las decisiones pendientes están en `README.md`.
- El siguiente paso es el inventario de archivos, descrito en `docs/04_archivo_y_busqueda.md`.

## Reglas de este proyecto

1. **Archivos.** Antes de mover, renombrar o borrar un archivo, se presenta un inventario y un plan. El responsable aprueba el plan. Cada movimiento queda en un registro que permite deshacerlo.
2. **Skills.** Las skills se construyen con el responsable. Él escribe la descripción y las reglas. Claude propone, escribe los guiones y ejecuta.
3. **Redacción.** Los documentos usan oraciones completas de hasta 25 palabras, en voz activa y sin tono de venta. Las celdas de las tablas siguen la misma regla.
4. **Documentos ligeros.** Si un documento queda denso, se recorta contenido. No se comprime el formato.
5. **Privacidad.** Este repositorio es público. No se suben datos personales, nombres de terceros, credenciales ni detalles de sistemas del trabajo. Ese material va en `privado/`, que git ignora.
6. **Antes de editar.** Se ejecuta `git pull`, porque el proyecto se trabaja desde dos computadoras.

## Dónde está cada cosa

| Qué | Dónde |
| --- | --- |
| Análisis y diseño | `docs/` |
| Evidencia y fuentes | `docs/anexos/` |
| Notas que no se publican | `privado/` (solo existe en la PC donde se creó) |
| Archivos de trabajo | Google Drive, carpeta `1_Comun` |
| Inventario de skills | Drive, carpeta `1_Comun\5_Skills` |
| Biblioteca | `D:\1_Lib` y el repositorio `biblioteca` |

## Método para guiones

El repositorio `biblioteca` contiene el método que ya funcionó: explorar, fichar, planificar, ejecutar y deshacer. Los guiones nuevos de inventario y de movimiento deben reutilizar ese método.
