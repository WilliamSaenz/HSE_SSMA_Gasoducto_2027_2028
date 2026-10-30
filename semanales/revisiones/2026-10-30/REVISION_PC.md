# Revisión de la planilla semanal de Planta Compresora — 30/10/2026

## Resultado

No se detectaron fórmulas rotas en la versión recibida. El recálculo completo de una copia, con LibreOffice Calc, terminó sin errores de celda (#REF!, #DIV/0!, #VALUE!, #NAME?, etc.). Hay pendientes de carga y de definición de períodos que impiden considerar cerrado el informe.

No se modificó el Excel recibido. La copia adjunta es idéntica byte por byte; no es una versión reparada ni el archivo convertido por LibreOffice. Se preservan las ediciones, nombres de hojas, datos, fotografías, gráficos, validaciones y formatos del usuario.

## Comprobaciones realizadas

- Archivo ZIP íntegro y XML legible; apertura con openpyxl y recálculo de una copia con Calc.
- 87 hojas; 437.416 celdas almacenadas, de las cuales 245.847 contienen fórmulas, incluidas fórmulas compartidas.
- Sin referencias explícitas #REF!, nombres definidos rotos ni referencias de fórmulas a hojas inexistentes. Los nombres nuevos 2,1 MAPs; 2,2 Observaciones-SMP; 03_TARJETAS_OBSERVACION y 04_FOTOS_SEMANA están vinculados.
- Relaciones internas del archivo válidas, coordenadas sin duplicados, rangos de validación y formato condicional válidos.
- Estructura de las 7 tablas consistente; 36 gráficos y 6 archivos de imágenes presentes. No se realizó revisión visual exhaustiva de cada gráfico ni prueba de hipervínculos web.
- Pruebas funcionales con fórmulas copiadas de esta versión, en archivos de prueba separados: 3/6 = 50%; 6/6 = 100%; SMP 6/6 + OPS 1/1 = 100% consolidado; 9/6 = 150%; sin personas aplicables = vacío. Se verificó que registros de septiembre, noviembre y personas no aplicables no inflan el porcentaje; un cierre semanal al 01/11 se limita al 31/10.
- El porcentaje superior de 01_SEGUIMIENTO_SEMANAL!K6 y el resumen K316 coinciden en las pruebas. Las metas permanecen SMP = 6 y OPS = 1 por persona y mes.

## Pendientes concretos

| Ubicación | Hallazgo | Acción necesaria |
|---|---|---|
| 01_SEGUIMIENTO_SEMANAL!C6:C7 | 01/10–11/10: período de 11 días | Confirmar si es un período acumulado deliberado o corregir con las fechas reales; no se redistribuyeron datos. |
| 01_SEGUIMIENTO_SEMANAL!E6:E7 | 18/10–25/10: período de 8 días | Confirmar las fechas reales. 05_COMPLEMENTO_PC marca REVISAR FECHAS y 06_PUENTE_MENSUAL_PC conserva N/D donde corresponde. |
| 2,2 Observaciones-SMP!C2:C7 y T2:T7 | Seis observaciones sin observador ni respuesta de alto potencial | Completar con información confirmada. La alerta V2:V7 funciona; los controles asociados de hallazgos también detectan datos faltantes. |
| 01_SEGUIMIENTO_SEMANAL!E224 y E225 | Dos acciones sin responsable | Asignar responsable y completar sus demás datos pendientes; N224:N225 actualmente informa el primer faltante. |
| 03_TARJETAS_OBSERVACION!A11:D130 | No hay universo nominal de personas que aplican | Completar nombres, empresas, cargos y Sí/No. Hay 113 tarjetas informadas (25 + 60 + 28), pero esos totales no permiten inferir el denominador ni el cumplimiento individual. El porcentaje vacío es correcto. |
| INICIO!C14 y C15 | Faltan analista y fecha de carga | Completar; DATA_QUALITY identifica ambos como errores de carga, no de fórmulas. |
| 05_COMPLEMENTO_PC y 06_PUENTE_MENSUAL_PC | Complemento e integridad de personas/eventos/hallazgos pendientes | Completar y confirmar únicamente con evidencia; los resultados N/D no deben sustituirse por cero. |

Las hojas históricas y auxiliares de control también muestran avisos por falta de registros, fotos o confirmaciones en sus propios módulos; no prueban corrupción del libro. El encabezado semanal indica “Revisar complemento PC” mientras el complemento está pendiente.

## Alcance y límites

Se verificaron estructura, referencias, recálculo y escenarios funcionales representativos. No se ejecutó Microsoft Excel de escritorio ni se certifica cada interacción de interfaz, conexión externa o salida a PowerPoint. La corrección factual de cifras y la completitud de fuentes necesitan revisión del responsable HSE. No se inventaron nombres, fechas, responsables ni datos de tarjetas.

SHA-256 del archivo recibido y conservado: `63fc75539296887c07fb5f738f0f26575b1586c05e633ddbb622167ecc37ee41`.
