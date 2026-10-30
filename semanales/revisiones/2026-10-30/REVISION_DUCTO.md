# Revisión y reparación de fechas — Semanal Ducto — 30/10/2026

## Resultado y entrega

Se repararon formatos de fecha y una referencia funcional del mes de tarjetas. El archivo resultante conserva los datos y las ediciones del usuario. El recálculo completo de una copia de prueba no produjo errores de celda. Persisten datos pendientes, que no se completaron sin evidencia.

Archivo: `plantillas/Planilla_Semanal_Ducto_V3_FECHAS_REVISADAS.xlsx`.

## Correcciones

- **01_SEGUIMIENTO_SEMANAL!E3:F3:** el serial 46296 era una fecha válida, 01/10/2026, presentada como General. Ahora se muestra como mes y año (`mmm yyyy`) y recupera el estilo amarillo de carga. No se cambió el valor ni el mes.
- **Fechas completas:** formato uniforme `dd/mm/yyyy` en campos que ya estaban definidos como fecha, incluidos inicios, cierres, vencimientos, observaciones, registros y hojas auxiliares. Los formatos que representan solo mes/año y los de duración se conservaron. También se formatearon las plantillas vacías para futuras cargas; no se convirtieron cantidades en fechas.
- **Corte de tarjetas:** 03_TARJETAS_OBSERVACION!Q5 y 01_SEGUIMIENTO_SEMANAL!C314:I314 muestran día/mes/año, no solo el mes.
- **03_TARJETAS_OBSERVACION!B4:** el mes de control ahora se obtiene de E3 de la hoja semanal. Antes se obtenía del comienzo de la primera semana, que puede pertenecer al mes anterior. La nueva fórmula fue probada con inicio 28/09 e informe de octubre: sigue mostrando octubre.
- Cálculo automático y recálculo completo al abrir; retirada coherente del índice de cálculo previo para que la aplicación lo reconstruya.

No se modificaron otros valores ni fórmulas. Se verificó esta conservación celda por celda; fuera de B4, las fórmulas permanecen intactas. Todas las partes no afectadas por las correcciones permanecen idénticas byte por byte, incluidos los 39 gráficos y los 15 archivos de medios.

## Verificaciones

- 78 hojas, 801.489 celdas almacenadas, 281.653 celdas con fórmulas (incluidas compartidas).
- ZIP íntegro, XML legible, apertura del archivo corregido, referencias internas del paquete y estilos válidos, coordenadas sin duplicados.
- No se encontraron referencias explícitas #REF!, nombres definidos con #REF! ni fórmulas que apunten a hojas inexistentes.
- Recálculo completo de una copia con LibreOffice Calc: **0 errores de celda**. Se entrega el archivo corregido preservando el formato original del paquete, no la copia convertida por LibreOffice.
- Pruebas con las fórmulas exactas de la entrega: 3/6 = 50%; 6/6 = 100%; 9/6 = 150%; sin personas aplicables = vacío. El resumen superior coincide con el detalle.
- Corte al 01/11 limitado al 31/10: no se suman tarjetas de noviembre. También se verificaron exclusión de septiembre, personas «No aplica» y comienzo de semana en el mes anterior.

## Pendientes que requieren datos o confirmación

No son corrupción del archivo ni fallas aritméticas. Los controles deben seguir mostrándolos.

- **Observaciones:** la columna V muestra como primer problema 76 registros sin contratista, 38 cerrados sin fecha de cierre y 38 con falta de gravedad. Los conteos son del primer aviso por registro; al completarlo podrían aparecer otros faltantes. Ver celdas en `PENDIENTES_DUCTO.csv`.
- **Semanal:** C42:E42 advierte faltantes de kilómetros; C85:E85 advierte faltantes de personal. Semanas 1–3 siguen «Incompleto»; semana 4, «Pendiente». No se sustituyeron vacíos por cero.
- **Períodos:** la semana 1 mantiene 01/10–11/10 (11 días). Confirmar si representa un corte acumulado deliberado o corregir las fechas con su respaldo. No se modificaron fechas reales ni se redistribuyeron los datos.
- **Tarjetas:** el porcentaje mensual necesita el listado nominal y la marca «Sí» en ¿Aplica? para las personas comprendidas. No se deduce la dotación ni el cumplimiento desde un total agregado.
- Los módulos históricos/auxiliares mantienen avisos de carga o de confirmación propios; la ausencia de errores de cálculo no implica que esos datos estén completos.

## Límites de la revisión

No se ejecutó Microsoft Excel de escritorio ni se certificaron enlaces externos, conexiones o salidas a PowerPoint. Las pruebas cubren estructura, recálculo y escenarios representativos; no certifican la veracidad de las cifras de origen. No se inventaron fechas de cierre, contratistas, responsables ni registros.

SHA-256 del archivo corregido: `01e9fa56440c54113b1c53f888e982d43a8fbe4d425f345c965353f2e665a15f`.
