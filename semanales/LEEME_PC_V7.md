# Semanal PC — V7 corregida

Usar [Planilla_Semanal_Planta_C_HSE_V7_CORREGIDA.xlsx](Planilla_Semanal_Planta_C_HSE_V7_CORREGIDA.xlsx) en reemplazo de V6.

La columna D del dataset `BD_CAPACITACIONES` decía **Tipo**, pero la definición de `tblBD_Capacitaciones` todavía decía **Fecha**. Se sincronizó la definición de la tabla con el encabezado. También se corrigieron los límites de las filas donde se agregó el selector semanal y la selección de la ventana para abrir en el registro de capacitaciones.

Se mantienen las tres opciones **Seguridad**, **Salud** y **Medio Ambiente**, y la semana se selecciona en O. Las celdas, fórmulas, validaciones, formatos y fotos son idénticos a V6; solo se corrigieron la definición interna de la tabla y metadatos de filas/visualización.

Verificaciones:

- 7 tablas: encabezados y columnas internas coinciden.
- 148 relaciones internas: destinos y referencias presentes.
- 84 hojas: sin fórmulas compartidas huérfanas.
- Límites de filas consistentes con las celdas de capacitación.
- Esquema Office 2021, SDK oficial Microsoft Open XML: 0 errores.
- Comparación con V6: todos los contenidos de celdas y fotografías conservados.

Estas comprobaciones no sustituyen una prueba de apertura directa en Excel LTSC, que no está disponible en este entorno.
