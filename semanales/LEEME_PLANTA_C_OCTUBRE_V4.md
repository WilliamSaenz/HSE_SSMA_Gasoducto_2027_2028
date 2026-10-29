# Semanal Planta C — octubre, V4: colores y verificación de datos

Archivo: `Planilla_Semanal_Planta_C_OCTUBRE_V4_COLORES.xlsx`.

Se conservó la V3 con los días trabajados en filas 64–66 y la carga manual de HH en fila 103: 195, 56 y 275; total 526 y tres semanas.

Único ajuste visual: Observaciones-SMP y MAPs adoptan la paleta de la captura: encabezados verde #92D050 con texto blanco, IDs amarillos, cuerpo blanco con cuadrícula gris, estado Cerrado verde claro y alertas de fecha rojas. Se conservaron las condiciones existentes de las alertas, los filtros, las validaciones, los anchos de columnas y los altos de filas. Las fechas de apertura y cierre se presentan como dd/mm/yyyy sin cambiar su valor.

Verificación contra `Planilla_Semanal_Planta_C_OCTUBRE.xlsx`, adjuntado originalmente:

- 87 hojas conservadas.
- 10.331 celdas constantes originales coincidentes después de tener en cuenta el traslado de filas. Las únicas diferencias de textos previas son A97 y A103, aprobadas para la nueva carga manual de HH.
- Sin datos originales eliminados o alterados; las seis imágenes del paquete original permanecen idénticas.
- Observaciones-SMP: 6 registros con ID en original y entrega. MAPs: 0 en ambos. La hoja 02_Observaciones-Desvios refleja esos mismos 6 registros.

El indicador preexistente de 230 observaciones cuenta las 230 fórmulas de A19:A248, incluso las que devuelven vacío; no representa 230 registros cargados. Se detectó y se informó, sin modificar esa fórmula en este cambio visual.

Respecto de V3, solo cambiaron las hojas Observaciones-SMP y MAPs y los recursos de estilo. Todos los valores y fórmulas de ambas hojas, así como los demás componentes, son idénticos. Se comprobaron la apertura de las 87 hojas mediante Apache POI, los colores de las celdas y la validez OOXML de hojas y estilos.
