# Semanal V12 — formato aprobado de observaciones

Archivo de entrega: `Planilla_Semanal_Ducto_V12_FORMATO_OBSERVACIONES_MENSUAL.xlsx`.

La base es el semanal XLSX aportado por el usuario: `Planilla Semanal Ducto_HSE_V2.xlsx`. Se conserva el libro semanal con sus 78 hojas. Únicamente la hoja `02_Observaciones-Desvios` adopta el formato, distribución, estilos, validaciones y tabla aprobados de `Observaciones-Desvios` del mensual `Plantilla_KPIs_Ducto_V5.xlsm`.

Se conservaron las 154 observaciones del semanal, cotejadas campo por campo. No se incorporaron los registros históricos del mensual. Empresa se ubicó en T e identificación HSE en W, según el formato aprobado. Los campos no informados permanecen vacíos. La semana y el mes del informe se conservan como auxiliares ocultos en X:Y. Las fórmulas del formato mensual toman el mes de `01_SEGUIMIENTO_SEMANAL!E3`.

Las otras 77 hojas son idénticas al semanal original. Se conservaron los componentes de ese libro y se agregaron únicamente los recursos de formato necesarios; se retiró la cadena de cálculo antigua para que Excel la regenere. No se copiaron macros del mensual a este XLSX.

Validación: apertura de las 78 hojas y recuento de 154 observaciones mediante Apache POI; tabla coherente de 22 columnas sin filtro de hoja superpuesto; encabezados del mensual verificados; comprobación de fórmulas de mes de apertura, semana y mes del informe; esquemas OOXML y referencias de estilos válidos.
