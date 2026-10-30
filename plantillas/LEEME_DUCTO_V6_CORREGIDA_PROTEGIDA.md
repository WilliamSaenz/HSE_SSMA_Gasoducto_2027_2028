# Mensual Ducto — V6 corregida, protegida y con Tarjetas libre

Archivo base: último Plantilla_KPIs_Ducto_V5.xlsm adjunto. Entrega: Plantilla_KPIs_Ducto_V6_CORREGIDA_PROTEGIDA.xlsm. Se mantuvo el formato XLSM y el proyecto VBA original.

## Cambios

- Rótulos de observaciones aclarados en dos filas, adaptados al Ducto: **UT+SMP**. La fila 29 tiene salto de línea y altura suficiente.
- Desglose por mes de apertura, sin arrastrar observaciones de meses anteriores. Agosto: 6 abiertas + 36 cerradas/positivas = **42**. Septiembre: 69 + 49 = **118**. Ambos totales coinciden exactamente con los valores manuales recibidos: no se perdieron ni agregaron observaciones.
- Se utiliza el registro de Observaciones-Desvios. Una positiva que también está cerrada se cuenta una sola vez. El KPI OBS y sus datos normalizados usan la suma de ambas filas, no solo abiertas. Los arrastres mantienen su indicador separado.
- Los meses sin registros o futuros se mantienen vacíos. Las filas ahora automáticas dejan de pedirse como carga manual en el control de completitud.
- Se repararon controles QA de texto vacío, decimales y conciliación de reporting: las celdas vacías de fórmulas no son datos inválidos ni ceros numéricos. Se conservaron los controles de calidad.
- Fechas completas normalizadas a dd/mm/aaaa, preservando los formatos de mes/año y las cantidades de origen. Se corrigió la guía de filas ART: cantidad en 61 y número de caso en 62.
- Tarjetas_Observacion: **la solapa existente queda totalmente sin protección**. Se conservaron su estructura, registros, fórmulas, meta y listas. Las instrucciones ahora señalan el selector correcto Datos!F1 y el alcance SMP en obra: inspectores IEBC, jefes de inspectores, coordinadores y gerente. No se crearon vínculos externos nuevos.
- El acumulado de tarjetas incluye el último día completo del mes, aunque un registro incluya hora.

## Protección

Las otras 63 hojas y la estructura del libro están protegidas con la clave indicada previamente por el usuario; no se reproduce en este documento. Las celdas originales de carga siguen editables. Se protegieron las fórmulas derivadas; se mantuvo editable la expresión manual de carga Datos!E13 (`32*9*31`), sin cambiar su cálculo. Para modificar el código, metas técnicas o estructura se necesita desproteger con la clave.

## Validación

- Apertura del XLSM, integridad ZIP, estado de protección, entradas editables y conservación del proyecto VBA comprobados.
- Recálculo independiente forzado de **213.229 celdas con fórmulas**, sin usar los resultados almacenados de la fuente: **0 errores de fórmula**. Los controles técnicos de texto, decimales y conciliación dan 0 / OK. Los controles QA no muestran errores de datos en el estado actual; las advertencias de información incompleta permanecen visibles.
- Los resultados calculados se actualizaron en el archivo original corregido sin sustituir sus fórmulas, imágenes, gráficos, macros ni protecciones por la copia convertida.
- Pruebas con las fórmulas exactas: abierta negativa, cerrada negativa, abierta positiva y cerrada positiva producen 1 abierta y 3 cerradas/positivas; con dotación 10, KPI = 0,4. Se verificó la exclusión de registros del mes anterior y el tratamiento de meses vacíos/futuros.
- Prueba de tarjetas: 6 tarjetas el último día del mes a las 15:00 producen 6 acumuladas y 100%; un registro del mes siguiente no se suma.
- Preservación comprobada de las entradas originales fuera del desglose nuevo. El proyecto VBA se conserva byte por byte. Su inspección estática confirma que el selector de fotografías usa Datos!F1 y una clave compatible con la protección aplicada. No se ejecutaron las macros ni Microsoft Excel de escritorio en este entorno.

## Uso y datos pendientes

Completar únicamente las celdas de carga. La ausencia de datos de octubre o del listado nominal de tarjetas no se reemplazó por cifras inventadas. Las advertencias y valores sin datos se mantienen; esta revisión verifica el funcionamiento técnico, no certifica la veracidad de cifras de origen ni las salidas a PowerPoint.

SHA-256 del XLSM entregado: `38771d843d80129c39ede6cf3a13b8589e7e1803a12ec5a40908a0dfdd81fd20`.
SHA-256 del proyecto VBA conservado: `d8446bd6f8ef129a9db29bc06d7c5d7d6e7dd3a80294c310c40fbc8f92989e8d`.
