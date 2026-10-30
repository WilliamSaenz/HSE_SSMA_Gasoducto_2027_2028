# Semanal Ducto corregida V2

Base exclusiva: último BORRADOR_Semanal_Ducto.xlsx aportado por el usuario. Se conservan sus datos y ediciones, sin reponer las filas eliminadas.

## Reparaciones

- Reparadas 198 fórmulas con referencias eliminadas y una regla de formato condicional dañada de 5.1 Microtrac 1!Z15:Z18.
- Kilómetros adaptados al formato actual: UT Proactivo + UT Geotab = UT; UT + SMP = consolidado. Los consolidados de livianos/pesados ahora esperan dos entradas y el total SMP suma sus dos categorías correctas. Los datos faltantes se siguen señalando y no se sustituyen por ceros.
- Controles de carga ajustados de 32 a 26 campos obligatorios por semana.
- Se dejaron vacíos 54 registros obsoletos de BD_SEMANAL que dependían del detalle eliminado: 36 de kilómetros y 18 de ICM. No se replica el agregado SMP como detalle por empresa. Los registros vigentes conservan sus fuentes.
- El control de escalas ICM considera los cuatro sistemas que mantienen entradas, en lugar de exigir los tres sistemas eliminados. Se conservan las escalas y datos originales.
- Las tarjetas mensuales y semanales se limitan al mes elegido aunque una semana cruce a otro mes. Se corrigen los avisos de fechas fuera del mes. Se mantiene el objetivo SMP de seis tarjetas por persona y mes y el alcance de personal en obra ya aclarado.
- Fórmulas compartidas expandidas a fórmulas individuales para evitar la estructura que Excel pidió reparar en la entrega anterior de Planta. Se conservan las fórmulas, capacidad de filas, objetos y resultados calculados; el archivo final no se convirtió mediante LibreOffice.
- Fechas completas en día/mes/año; se mantienen los formatos de mes y hora. La hoja 03_TARJETAS_OBSERVACION queda sin protección; las demás y la estructura usan la clave acordada, conservando editables las celdas de carga existentes.

## Verificación y límites

78 hojas y 281.590 fórmulas. Recálculo completo independiente en copia temporal, sin errores de celda. Pruebas de suma UT/SMP, kilómetros faltantes, 26 campos completos, tarjetas fuera del mes, exclusión de personas que no aplican y carga en la última fila 1510 satisfactorias. Se conservaron los datos literales del usuario salvo el rótulo del número de campos obligatorios; imágenes y objetos preservados.

No hay vínculos a libros externos ni conexiones externas de datos. Los hipervínculos normales a SharePoint se conservan. Se actualizó el paquete de cuatro planillas V6; este no implica nuevas modificaciones a los otros tres archivos.

Preparada para cargar en SharePoint. No se realizó una carga/descarga real en ese servicio por falta de inicio de sesión ni una apertura con Microsoft Excel de escritorio. Los controles siguen señalando los datos pendientes o inconsistentes: no se inventaron valores para ocultarlos.
