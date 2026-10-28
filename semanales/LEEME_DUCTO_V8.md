# Planilla Ducto V8 — reemplaza V6 y V7

Archivo vigente para esta revisión: `Planilla_Semanal_Ducto_HSE_V8_CORREGIDA.xlsx`.

El informe de reparaciones de Excel identificó la eliminación del filtro y de la tabla `xl/tables/table1.xml`. Se sustituyó ese objeto de tabla por un rango normal con autofiltro en A18:X248, conservando el formato y todos los registros. No existen fórmulas dependientes de `tblObservaciones`. Se actualizaron las relaciones y el tipo de contenido del paquete y se registró el rango del filtro en el libro.

También se corrigieron 213 referencias a estilos base inexistentes, presentes en los estilos importados. Cada formato de celda conserva sus fuentes, rellenos, bordes, alineaciones y formatos numéricos explícitos.

Comprobaciones realizadas:

- Los datos y fórmulas de las 78 hojas son idénticos a V7; se comparó el contenido `sheetData` de todas las hojas.
- Auditoría de 694.437 celdas: índices de estilos, referencias de estilos base y destinos de relaciones válidos.
- Apertura de las 78 hojas con Apache POI 5.4.1; las 6 tablas restantes tienen dimensiones y definición de columnas consistentes.
- Validación OOXML de estilos, seguimiento y observaciones, separando las extensiones de Microsoft solo en la vista de validación.
- Comprobación de las sumas de HH: semana 1 = 83; semana 2 = 349; semana 3 = 102; total = 534 HH.

Microsoft Excel no está disponible en el entorno de validación. La comprobación de apertura se realizó con un lector independiente. Se conservan los originales y las versiones anteriores como antecedentes.
