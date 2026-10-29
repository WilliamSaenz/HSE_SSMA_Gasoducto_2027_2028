# Semanal Planta C — octubre, V2

Archivo: `Planilla_Semanal_Planta_C_OCTUBRE_V2_DIAS_REUBICADOS.xlsx`.

Base exclusiva: `Planilla_Semanal_Planta_C_OCTUBRE.xlsx`, adjuntado por el usuario. Se mantiene el formato propio de Planta C; no se adapta al formato del Ducto.

Único cambio de distribución solicitado: trasladar el bloque DÍAS TRABAJADOS de las filas 86–88 a las filas 64–66, inmediatamente después de la fila 63. La fila 64 contiene el título, la 65 corresponde a OPS y la 66 a SMP (IEBC + YPF + PAE). Las filas originales 64–85 bajan tres posiciones. Las filas posteriores a la 88 conservan su posición.

Se ajustaron referencias de fórmulas, rangos, validaciones, formatos condicionales y comentarios. También se actualizaron referencias dependientes en otras hojas. La cadena de cálculo anterior se retiró para regenerarse al abrir el archivo; las fórmulas compartidas del seguimiento se escribieron individualmente al mover las filas.

Verificación: las 87 hojas abren mediante Apache POI. Se conservaron las 2.462 celdas sin fórmulas del seguimiento y los datos constantes de las otras hojas. El archivo de estilos y todas las imágenes permanecen idénticos al original. El esquema OOXML de seguimiento es válido. Pruebas en memoria confirmaron la carga editable de días en OPS/SMP, el conteo de semanas, la independencia de los totales de HHT frente a los días y el cálculo de cumplimiento de comités desplazados. Los valores de prueba no se guardaron en el archivo entregado.
