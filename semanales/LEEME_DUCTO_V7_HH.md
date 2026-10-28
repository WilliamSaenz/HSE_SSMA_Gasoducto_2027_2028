# Planilla ducto V7 — corrección de apertura

Archivo: `Planilla_Semanal_Ducto_HSE_V7_COMPATIBLE_EXCEL.xlsx`.

Sustituye a `Planilla_Semanal_Ducto_HSE_V6_HH_SEMANALES.xlsx`, que produjo un aviso de recuperación en Microsoft Excel.

Se corrigió la definición interna de `tblObservaciones`: el rango A18:X248 tiene 24 columnas, pero la V6 declaraba solamente 22. La V7 declara las 24 columnas, con identificadores consecutivos y nombres coincidentes con los encabezados. Todos los demás componentes del archivo se conservaron byte por byte, incluidos datos, fórmulas y formatos.

Validación realizada:

- Apertura de las 78 solapas mediante Apache POI 5.4.1.
- Coincidencia de rango y definición de columnas en las 7 tablas del libro.
- Validación de los esquemas OOXML de estilos, seguimiento semanal, observaciones y tabla; las extensiones de Microsoft se excluyeron únicamente de la vista de validación del esquema base y se conservaron en el archivo entregado.
- Comprobación independiente de las sumas de HH: semana 1 = 83, semana 2 = 349, semana 3 = 102; total = 534 HH.
- Verificación de que el único componente modificado respecto de V6 es `xl/tables/table1.xml`.

No se dispone de Microsoft Excel en este entorno; la apertura se verificó con un lector independiente. Se conservan las instrucciones de recálculo completo al abrir en Excel.
