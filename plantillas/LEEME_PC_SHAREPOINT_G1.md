# Planta Compresora lista para carga en SharePoint — enlace de fotos en G1

Base: último archivo Plantilla_KPIs_PC_TARJETAS_LIBRE.xlsx aportado por el usuario. Entrega: Plantilla_KPIs_PC_SHAREPOINT_G1.xlsx.

- Se movió la fórmula del enlace de fotos de Datos!W1 a G1, con la combinación G1:AL1. W1 quedó vacío; no se eliminaron columnas ni se desplazó la matriz mensual.
- Se encontró un vínculo de libro externo en Tarjetas_Observacion!N4: apuntaba a la hoja Observaciones-Desvios de un libro del Ducto. Esa era una dependencia real capaz de provocar el aviso de actualización.
- Se reemplazó por el conteo de las fechas del registro local Observaciones-SMP de Planta, desde el inicio hasta el fin completo del mes seleccionado. Octubre devuelve 3, igual al conteo independiente de las filas del registro.
- Tras sustituir la fórmula, se eliminaron el externalLink, su caché del libro ajeno, su relación y su declaración de contenido. La entrega no tiene referencias a otros libros ni partes externalLinks. No se ocultaron avisos ni se congeló el contador: sigue siendo automático.
- La pestaña de tarjetas copiada del Ducto ahora dice Planta Compresora, señala Datos!F1 como selector y genera el frente Compresora en sus registros. Se mantiene la meta suministrada de 6 tarjetas y el alcance SMP. Se incluyó todo el último día del mes aunque una fecha contenga hora.
- Se preservaron las protecciones y todos los registros; Tarjetas_Observacion continúa sin protección de hoja. Los avisos por fechas de cierre pendientes/incoherentes y falta de exposición de octubre no se borraron ni completaron con datos inventados.
- Archivo íntegro y recálculo forzado de una copia sin resultados almacenados: cero errores de fórmula. Se actualizaron los resultados de la entrega manteniendo sus fórmulas, formatos, dibujos y protecciones originales.

La carga y descarga real en SharePoint siguen sin comprobarse por falta de inicio de sesión. El archivo está preparado sin dependencias de cálculo a libros en rutas locales. El paquete V2 contiene esta mensual actualizada y las otras tres planillas de la entrega anterior.
