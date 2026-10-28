# Planilla Ducto V9 — carga horizontal por semana

Archivo: `Planilla_Semanal_Ducto_HSE_V9_CARGA_HORIZONTAL.xlsx`.

- Días trabajados: una única fila, C16:F16, alineada con SEM. 1 a SEM. 4. Las antiguas filas 17 a 20 se eliminaron. I16 acumula los días cargados; J16 cuenta las semanas con dato.
- HH de capacitación: carga manual horizontal en C120:F120. Es la antigua fila 124, que subió cuatro posiciones por la eliminación de filas. Se conservaron las HH disponibles: 83, 349 y 102; la semana 4 queda vacía.
- El resumen de HH de capacitación y el acumulado mensual toman los valores manuales de esa fila. El detalle existente queda como respaldo opcional, con sus datos conservados. El control inmediato anterior coteja el desglose del detalle con la carga semanal.
- Se ajustaron fórmulas, validaciones, rangos y referencias de las otras hojas afectadas por el desplazamiento. También se ajustaron las posiciones de comentarios heredados.
- Observaciones conserva el rango con filtros de V8; no se reintrodujo el objeto de tabla rechazado por Excel.

Validación: apertura con Apache POI de las 78 hojas; entradas semanales desbloqueadas y sin combinaciones; total de HH 534. Pruebas en memoria con cambios manuales, decimales, ceros y blancos demostraron que los resúmenes y acumulados responden a la carga horizontal. Los datos de prueba no se guardaron en el archivo entregado. Se comprobaron los esquemas OOXML de estilos y hojas editadas, la conservación de los datos digitados existentes y la ausencia de referencias de estilo inválidas.

Microsoft Excel no está instalado en el entorno: la apertura y los cálculos se verificaron mediante un lector independiente.
