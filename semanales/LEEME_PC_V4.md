# Semanal HSE de Planta Compresora — V4

La versión V4 conserva el archivo semanal recibido y agrega cobertura de las entradas del mensual, con Observaciones-SMP y MAPs en el formato de la mensual adjunta `Plantilla_KPIs__PC_V5.xlsx`.

## Carga semanal del analista

1. **01_SEGUIMIENTO_SEMANAL:** mantener fechas y registros operativos. Revisar las fechas existentes: la primera semana cargada abarca 1–11/10/2026 (11 días) y la última cruza a noviembre. Se señalaron; no se cambiaron sin evidencia.
2. **Observaciones-SMP / MAPs:** una fila por registro, con ID único. Las columnas A:T coinciden con las de la mensual: títulos, orden, anchos, fuentes, colores y desplegables. Las primeras tres columnas y el encabezado quedan inmovilizados; filtrar por semana U y estado O. Campos blancos editables; ID amarillo como la mensual. U/V/Y son automáticos. W/X sugieren gravedad y cantidad de detenciones y pueden corregirse con evidencia. No duplicar el registro cada semana: actualizar estado, cierre y evidencia en la misma fila.
3. **03_FOTOS_SEMANA:** conservar las fotos originales y completar lugar, descripción, estado y período verdadero. Hay dos espacios por cada una de seis semanas; no se inventó material faltante.
4. **05_COMPLEMENTO_PC:** combis por empresa, días trabajados 0–7, positivos de tests, campañas y OCS. Los datos operativos existentes se sugieren automáticamente cuando toda la semana pertenece al mes. Si cruza meses, cargar la porción real, sin prorratear horas ni kilómetros por cantidad de días.
5. **07_PERSONAS_PC:** ID estable por persona y semana, días en campo, HHT y HH de formación. Permite contar personas distintas sin sumar asistentes repetidos. Documentar la base de días de la dotación promedio.
6. **08_EVENTOS_PC:** los accidentes de personal y vehiculares se enlazan desde 01. Completar N° ART y categoría IOGP cuando corresponda; las investigaciones se cargan desde la fila 30 con fechas de origen y cierre. No volver a digitar los accidentes.
7. **06_PUENTE_MENSUAL_PC:** revisar resultados por fila destino del mensual y confirmar integridad de los registros. N/D significa pendiente, no cero. Abiertos se calculan a fecha de corte, incluyendo arrastres; nunca sumando stocks semanales. Las observaciones estándar/positivas no se cuentan como desvíos. **10_CONTRASTE_PC** documenta la comparación y las reglas.

## Cobertura adicional

ICM por sistema/empresa se conserva en 01 (no sumar ni promediar escalas distintas). Se incluyen kilómetros de livianos, pesados y combis; días trabajados; tests de alcohol y drogas y sus positivos; acciones abiertas y futuras; fotos de actividades relevantes; y las clasificaciones, fechas y registros necesarios para deducir las entradas mensuales. Los KPIs finales continúan calculándose en la mensual.

El apoyo 09 es automático y queda oculto para evitar doble digitación. Se conserva la hoja legada de observaciones y una copia íntegra de su versión recibida; el registro legado no contenía filas de detalle cargadas, aunque sí un total manual semanal de 7, que se conservó sin inventar registros. Los datos históricos de la mensual se usaron como referencia de estructura, no se copiaron al semanal como datos actuales.

## Verificación

- Comparación OOXML: fotografías y objetos enriquecidos preservados; ninguna eliminación de hojas originales.
- Ambas solapas tienen 1.000 filas y los mismos 20 encabezados y anchos A:T de la mensual. Se conservaron los 13 desplegables extendidos de cada solapa y sus catálogos.
- Se verificó que las entradas son editables, que las fórmulas auxiliares están bloqueadas y que los filtros están habilitados.
- Se recalcularon escenarios sintéticos válidos e inválidos con LibreOffice: personas repetidas, capacitación, corte mensual, ART de accidente anterior, investigaciones, stock de hallazgos, MAPs y desvíos, semanas de más de 7 días, positivos mayores que tests, cierre sin fecha e ID duplicado entre solapas.
- Se revisaron visualmente las dos tablas con datos sintéticos; estos datos de prueba no están incluidos en el entregable.
- Las pruebas validan la plantilla y sus reglas; los datos reales pendientes y las fechas señaladas requieren completarse y revisarse antes de emitir un mensual.

## Trazabilidad

- Semanal recibido: `Planilla Semanal Planta_C_HSE_V2.xlsx` — SHA256 `52678b08a4803f9d8274fd40e6fa4d4c449842679e8a5761291408a9c4c5829d`
- Mensual de referencia adjunta: `Plantilla_KPIs__PC_V5.xlsx` — SHA256 `87315ea71aeb8109c1050c35948c426eb517100a4fd7cef527d36ed52c9a196c`
- Entregable: `Planilla_Semanal_Planta_C_HSE_V4_FORMATO_MENSUAL.xlsx` — SHA256 `c7d0c92cb26c7ca2b3a85610e4d35a0107b62824db27dfc3e9650531b5b0a0dd`
