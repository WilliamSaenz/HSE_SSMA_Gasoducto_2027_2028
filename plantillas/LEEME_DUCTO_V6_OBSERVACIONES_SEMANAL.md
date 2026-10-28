# Observaciones del semanal incorporadas al mensual aprobado

Archivo: `Plantilla_KPIs_Ducto_V6_OBSERVACIONES_SEMANAL.xlsm`.

Base: último mensual aportado por el usuario, `Plantilla_KPIs_Ducto_V5.xlsm`. Origen: solapa `02_Observaciones-Desvios` del último `Planilla Semanal Ducto_HSE_V2.xlsx` aportado.

Se incorporaron sus 154 observaciones en las filas 179 a 332 de `Observaciones-Desvios`, conservando las 160 observaciones históricas del mensual. Total: 314 registros, sin coincidencias de ID entre ambas fuentes. Se respetó el formato mensual aprobado, incluyendo estilos, validaciones, tabla y fórmulas. Empresa pasó de W del semanal a T del mensual; identificación HSE pasó de X a W. Los campos no informados no se completaron con datos inventados. Se ajustó el alto de las nuevas filas para sus textos.

Verificación: comparación campo por campo de los 154 registros; conservación íntegra de las filas históricas; apertura de las 64 hojas con Apache POI; tabla de observaciones coherente; fórmulas de mes de apertura verificadas para filas nuevas. El proyecto VBA y todos los componentes del mensual son idénticos al original, salvo la hoja de observaciones y la instrucción del libro para recalcular al abrir.

SHA256 del proyecto VBA, idéntico en original y entrega: `e6ae1e84fa7bf3dd5ae8d0d91df0473b0d907b8f6246b6dc64f92ad670fece14`.
