# Anexo D. Lo que Claude puede hacer sin supervisión

**Fecha de verificación:** 25 de noviembre de 2026. Los datos vienen de la documentación oficial de Claude. Varias funciones están en vista previa y sus límites pueden cambiar.

## Resumen

| Capacidad | ¿Funciona con la PC apagada? | Dónde corre |
| --- | --- | --- |
| Tarea programada en la nube | Sí | Una máquina de Anthropic, con una copia nueva del repositorio en cada corrida |
| Tarea programada de Cowork sin carpeta local | Sí | La nube de Anthropic |
| Tarea programada de Cowork con carpeta local | No | La PC, con la aplicación abierta |
| Tarea programada de la aplicación de escritorio | No | La PC, con la aplicación abierta |
| `/loop` y tareas de sesión | No | La terminal, con la sesión abierta |
| `claude -p` lanzado por el programador de Windows | No documentado | La PC |
| Claude in Chrome | No | El navegador del usuario |
| Uso de computadora en Windows | No | La PC, con la aplicación abierta |
| Agente administrado con despliegue programado | Sí | Un entorno de Anthropic, pagado con créditos de API |
| Iniciar sesión en un sitio web y descargar, en la nube | No documentado | — |

## Tareas programadas en la nube

Fuentes: <https://code.claude.com/docs/en/routines.md> y <https://code.claude.com/docs/en/cloud-environments.md>

- Corren en la infraestructura de Anthropic, aunque la computadora esté apagada.
- Tienen tres disparadores: un horario, una llamada por API y un evento de GitHub.
- El intervalo mínimo es de una hora.
- Cada corrida empieza con una copia nueva del repositorio. Los procesos no persisten entre corridas.
- La red puede ser limitada o completa. La red completa permite llegar a cualquier sitio.
- Cada corrida puede usar los conectores configurados, como Notion o Drive.
- Las corridas consumen el mismo límite de uso que las sesiones interactivas.
- La documentación no confirma la búsqueda web dentro de una corrida.
- La documentación no describe un navegador manejado por Claude dentro de una corrida.

## Opciones que exigen la PC encendida

Fuentes: <https://code.claude.com/docs/en/desktop-scheduled-tasks.md>, <https://code.claude.com/docs/en/scheduled-tasks.md> y <https://code.claude.com/docs/en/chrome.md>

- Las tareas de la aplicación de escritorio corren solo con la aplicación abierta y la computadora despierta.
- `/loop` y las tareas de sesión corren solo mientras la sesión está abierta.
- Claude in Chrome usa la sesión iniciada del navegador del usuario. Se detiene ante una pantalla de ingreso o un CAPTCHA y pide ayuda.

## Agentes administrados

Fuentes: <https://platform.claude.com/docs/en/managed-agents/overview> y <https://platform.claude.com/docs/en/managed-agents/scheduled-deployments>

- Son agentes que corren en un entorno de Anthropic, con terminal, archivos, búsqueda web y conectores.
- Sus sesiones conservan los archivos y el historial.
- Admiten despliegues programados con precisión de minutos.
- Cuestan los tokens del modelo más US$ 0,08 por hora de sesión activa.
- Los créditos de API del plan Max pueden pagar este servicio.

## Conclusión

Claude cubre los encargos programados y la búsqueda en la web abierta. Claude no ofrece hoy una computadora persistente que inicie sesión en sitios web con la PC apagada. Esa función justifica mantener un agente en la nube de otro proveedor.
