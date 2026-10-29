# Semanal Planta C — octubre, V3

Archivo: `Planilla_Semanal_Planta_C_OCTUBRE_V3_HH_MANUALES.xlsx`.

Base: V2 de Planta C con DÍAS TRABAJADOS debajo de fila 63. Ese bloque y los demás cambios se conservan.

La fila 103 se reemplazó por carga manual horizontal de HH de capacitación. A103: HH de capacitación por semana; B103: TOTAL · carga manual. C103:H103 quedan editables y sin combinaciones; I103 acumula y J103 cuenta semanas con datos. Por confirmación expresa del usuario se conservaron las cifras de Planta C: 195, 56 y 275, total 526 y tres semanas; no se copiaron las cifras de la captura del Ducto.

El resumen de HH en la fila 97 ahora toma los valores de la fila 103. Los resultados dependientes, incluida BD_SEMANAL, responden a esa carga manual. Se conserva el registro detallado, las fuentes originales y el catálogo de semanas oculto R99:R104; R103 sigue conteniendo 5. Se mantiene el formato de Planta C y se grisan las semanas sin fechas según su regla de formato existente.

Validación: apertura de las 87 hojas con Apache POI; total 526, tres semanas; pruebas en memoria con edición de HH, decimales, cero y blanco; actualización del resumen y de BD_SEMANAL; bloque de días y catálogo de semanas conservados. Los datos de prueba no se guardaron. Se compararon todos los componentes no afectados y las celdas ajenas al cambio; se validaron los esquemas OOXML de la hoja y los estilos.
