# Planilla Ducto V11 — días trabajados debajo de fila 80

Archivo: `Planilla_Semanal_Ducto_HSE_V11_DIAS_REUBICADOS.xlsx`.

El bloque DÍAS TRABAJADOS se retiró de las filas 15 y 16 y se ubicó en las filas 81 y 82. Los valores semanales se cargan en C82:F82; I82 acumula los días y J82 cuenta las semanas con dato. La carga horizontal de HH de capacitación permanece en C120:F120. Las columnas auxiliares R:U siguen ocultas.

Se reajustaron las referencias de fórmulas, rangos, validaciones, formatos condicionales y comentarios. La suma de HHT utiliza únicamente las filas de empresas (78:80 y 83), excluyendo las dos filas del bloque trasladado.

Verificación: apertura de las 78 hojas mediante Apache POI; carga horizontal editable; total de HH de capacitación conservado en 534. Pruebas en memoria comprobaron la suma semanal de días y la independencia del total de HHT respecto de los días digitados. Los valores usados en las pruebas no se guardaron. Se comprobaron la conservación de 3.141 celdas sin fórmulas, la validez OOXML de la hoja y la conservación íntegra de observaciones.
