# Mensual Planta Compresora — V6 corregida y protegida

Se trabajó sobre el último archivo del usuario, Plantilla_KPIs__PC_V5.xlsx. Archivo entregado: Plantilla_KPIs_PC_V6_CORREGIDA_PROTEGIDA.xlsx.

## Reparaciones y criterio de observaciones

- Se conectaron las filas nuevas Datos 28 y 29: abiertas, y cerradas/positivas. Se consideran observaciones originadas en cada mes según su estado cargado, sin arrastres. Los pendientes de meses anteriores tienen su indicador separado de hallazgos abiertos a fin de mes (Datos fila 69).
- OPS utiliza el detalle ya existente de las filas 64 y 65; SMP utiliza el registro Observaciones-SMP. No se suma nuevamente la hoja MAPs sobre el detalle manual de OPS, para evitar duplicados.
- Las positivas que también están cerradas se cuentan una sola vez. Las clasificaciones estándar, positivas y buenas prácticas se agrupan como positivas; las subestándar no se confunden con estándar.
- El KPI OBS y sus datos normalizados suman ambas filas; el indicador de completitud deja de pedir carga manual en las filas ahora automáticas. Ejemplo con los datos actuales: septiembre = 86 abiertas + 91 cerradas/positivas = 177; el cociente usa la dotación promedio de ese mismo mes. No se recuperaron cifras borradas del archivo anterior.
- Se corrigieron tres controles QA: cadenas vacías generadas por fórmulas ya no se cuentan como texto ingresado; el control de decimales ya no produce -1 ante celdas vacías; la conciliación con reporting compara valores y tipos numéricos reales en lugar de tratar vacíos como ceros.
- Fecha de cierre Observaciones-SMP!S65: el texto 26/92026 se normalizó a 26/09/2026. Las fechas dudosas no se inventaron ni desplazaron.
- Se normalizaron formatos de fecha completos y se actualizó la indicación de edición de metas: la columna C de KPIs es automática y no debe sobrescribirse.

## Protección y uso

Las 60 hojas y la estructura del libro están protegidas con la clave indicada por el usuario, que no se reproduce en este documento. No es un archivo cifrado con contraseña de apertura.

Todas las fórmulas quedaron bloqueadas, incluidas 38 que antes eran editables. Las celdas de carga originales siguen desbloqueadas: selector de mes Datos!F1, entradas numéricas de Datos, registros de Observaciones-SMP y MAPs, catálogos y campos de fotos que ya permitían entrada. Las hojas de fotos permiten editar objetos. Para cambiar fórmulas, estructura o metas técnicas se requiere desproteger con la clave.

## Validación

- Apertura, integridad ZIP y lectura de la protección y su contraseña verificadas.
- Recálculo independiente forzado de las 76.093 celdas con fórmulas: se eliminaron los resultados almacenados de una copia temporal antes de calcular con LibreOffice Calc. Resultado: cero errores de celda.
- Se actualizaron los resultados almacenados de la entrega con ese cálculo, sin reemplazar sus fórmulas, validaciones, imágenes, gráficos ni protecciones por la versión convertida.
- Pruebas con fórmulas exactas: 4 observaciones SMP (abierta negativa, cerrada negativa, abierta positiva y cerrada positiva) más OPS 3 abiertas y 2 positivas producen 4 abiertas + 5 cerradas/positivas = 9, sin doble conteo. Con dotación 10, KPI = 0,9. Otros meses se excluyen; meses futuros o sin registros y sin detalle manual permanecen vacíos.
- Contraseña de las hojas y estructura, bloqueo de todas las fórmulas y edición de entradas verificados programáticamente. No se ejecutó Microsoft Excel de escritorio.

## Datos pendientes reales

Estos avisos continúan visibles en _QA y Control. No implican fórmulas rotas, pero impiden dar por cerrado el reporte:

- 15 observaciones cerradas sin fecha de cierre: S37, S39, S41, S42, S43, S45, S46, S48, S50, S52, S53, S54, S69, S70, S71 de Observaciones-SMP.
- 2 fechas de cierre anteriores a la apertura: S34, S61. Incluye un año 2006 frente a una apertura en 2026 y un cierre del 22/09 frente a apertura del 23/09; se requiere confirmar cuál fecha es correcta.
- 4 fechas de cierre que no son fechas válidas: S55, S56, S58, S59. Textos como SI/si o un año 206 necesitan confirmación.
- Un KPI tiene observaciones registradas en octubre sin la dotación/exposición de octubre cargada. El cociente se mantiene sin valor y el control conserva el aviso; no se convirtió el faltante en cero.
- Persisten advertencias de carga de octubre, snapshots históricos, fuentes/metas y fotografías sin descripción.

SHA-256 de la entrega: `2887ed32cafe5531038492b819c36ef67affbbebcb3dece0664ac2cdf46f4b9f`.
