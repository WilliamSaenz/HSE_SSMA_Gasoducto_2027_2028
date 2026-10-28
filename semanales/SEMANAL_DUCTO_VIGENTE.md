# Semanal Ducto — versión integrada vigente

Archivo vigente: [Planilla_Semanal_Ducto_V15_INTEGRADA_EMPRESA.xlsx](Planilla_Semanal_Ducto_V15_INTEGRADA_EMPRESA.xlsx?raw=true).

La V15 conserva íntegra la V14 y cambia únicamente el encabezado T18 de observaciones a **Empresa**. Se verificó que B122 sigue siendo **Tipo** y B123:B192 mantiene el desplegable Seguridad / Salud / Medio Ambiente, con celdas desbloqueadas. Datos, fórmulas, fotografías y demás hojas no cambiaron.

La V14 reúne los cambios aprobados que quedaron separados al usar un adjunto anterior como base de V12. Para nuevas ediciones, conservar este conjunto completo; si el usuario aporta un archivo más reciente, cotejarlo y preservar sus cambios sin perder estas funcionalidades.

## Funcionalidades conservadas

- DÍAS TRABAJADOS en filas 81 y 82; carga horizontal C82:F82 bajo SEM. 1 a SEM. 4. I82 acumula y J82 cuenta semanas con dato.
- HH de capacitación manuales en C120:F120; se conservan 83, 349 y 102 HH. Total disponible: 534. Los resúmenes semanales y mensual toman esa fila.
- Tipo de capacitación en B del detalle: Seguridad, Salud y Medio Ambiente. El detalle histórico queda como respaldo opcional; se conservan las fechas y valores cargados.
- Columnas auxiliares R:U ocultas en seguimiento.
- Las 154 observaciones del semanal mantienen el formato aprobado del mensual. El rango tiene filtros y no contiene el objeto de tabla que produjo reparaciones en Excel. No se incorporan los 160 registros históricos del mensual a este semanal.
- Ocho fotos convencionales: dos de semana 1, tres de semana 2 y tres de semana 3. Se preservan los bytes originales de las fotos y sus descripciones. Falta la foto del Tramo Sur de la semana 1 en las fuentes disponibles.

## Controles corregidos

Los siete avisos tratados antes como errores eran HH faltantes en registros del detalle opcional. Los controles ahora separan pendientes opcionales de valores inválidos. En los datos entregados, las semanas 1–3 muestran respectivamente 12, 25 y 9 pendientes opcionales; no se completaron con valores inventados. Los controles de observaciones del formato mensual permanecen activos.

Se mantienen errores reales por HH negativas, valores no numéricos, semanas fuera de rango y tipos fuera del catálogo. La carga semanal manual de HH tiene su propio control; una semana sin HH se informa como pendiente. Los errores y avisos no se fuerzan a cero: los contadores siguen vinculados a los datos.

## Verificación de integración

- Conservación de 3.141 celdas sin fórmulas de la hoja de seguimiento y de todos sus estilos base. Las únicas modificaciones adicionales de esa hoja son controles de calidad coherentes con la carga manual y la altura de la fila del resumen de controles.
- Conservación íntegra de los datos y fórmulas de las observaciones de V13, con remapeo seguro de estilos.
- Conservación de la hoja y los dibujos de fotos de V13; ocho anclajes comprobados con Apache POI.
- Apertura de las 78 hojas; las otras 75 hojas permanecen idénticas a V11.
- Pruebas en memoria de carga de días, HH, decimales, ceros, blancos, HH negativas y tipo inválido. El total de HHT excluye las filas de días trabajados. Ningún valor de prueba se guardó en el entregable.
- Validación OOXML de estilos y de las tres hojas relevantes; índices de estilos, destinos de relaciones e identificadores de tablas coherentes. No se reintroduce `xl/tables/table1.xml`.

Microsoft Excel no está disponible en el entorno; las pruebas de apertura y cálculo se hicieron con un lector independiente. V12 y V13 quedan como antecedentes parciales; usar V15 integrada para continuar.
