# Ducto — corrección de carga y optimización V2

Se trabajó sobre el último Mensual_Ducto.xlsm aportado por el usuario. Entrega: Mensual_Ducto_CORREGIDO_V2.xlsm.

## Hallazgo confirmado

El archivo era íntegro y no tenía vínculos externos ni errores de celda guardados. Contiene 64 hojas y 213.229 fórmulas. Estaba configurado para forzar un recálculo completo al abrir. Solo _FIND_DS ocupaba 26,25 MB de XML y 121.500 fórmulas, muchas con búsquedas repetidas de los mismos campos. Es una carga relevante al abrir y al actualizar datos. No se reproduce en este entorno un diálogo de reparación de Microsoft Excel, que no está instalado aquí.

## Cambios aplicados

- Se sustituyeron **139.500 búsquedas INDEX/MATCH repetidas** por referencias directas equivalentes a las columnas reales del formulario. Los campos se resolvieron contra los encabezados de esta última versión. Excel sigue actualizando referencias al mover columnas mediante sus funciones normales; cualquier reorganización mediante herramientas externas debe volver a validarse.
- Se sustituyeron **22.500 escaneos de longitud de filas** por comprobaciones ligeras de las celdas de entrada. Se evitó que esas comprobaciones dependan de columnas automáticas de días y control.
- Se optimizaron 76.500 celdas de fórmulas sin reducir las 4.500 filas de observaciones, los 5.000 registros de tarjetas ni los meses del calendario.
- Se mantuvo **cálculo automático**, quitando la obligación de recálculo global en cada apertura. Los cambios de datos continúan calculándose; se conserva el cálculo antes de guardar. Se entregan resultados almacenados ya recalculados y comprobados.
- Se conservó la navegación de fotos en Datos!G1, el selector Datos!F1, Tarjetas_Observacion sin protección, las demás protecciones y la estructura. No se cambió la clave.

Tamaño recibido: 4,787,428 bytes. Tamaño final: 3,676,152 bytes. Reducción: **23.2%**. El tamaño y el trabajo repetido disminuyen; no se promete un tiempo concreto de apertura en otros equipos.

## Validaciones realizadas

1. ZIP/XML, relaciones internas, coordenadas sin duplicados, índices de estilos/cadenas y rangos combinados: correctos en las 64 hojas.
2. Recálculo independiente forzado de dos copias, antes y después, eliminando sus resultados almacenados para que se vuelvan a calcular.
3. Comparación de **91,133 valores calculados**: **cero diferencias**, con tolerancia numérica relativa de 1e-11 para decimales. **Cero errores de fórmula**.
4. Prueba funcional en una copia temporal: se añadió una observación negativa abierta y dotación 11 para octubre. El auxiliar recibió el registro, el mensual indicó 1 abierta y 0 cerradas/positivas y el KPI dio 1/11. La entrega no contiene ese registro ni esos datos de prueba.
5. Comparación final de los resultados almacenados de la entrega contra la copia anterior recalculada: nuevamente cero diferencias. Los totales originales de agosto y septiembre permanecen 42 y 118.
6. Todos los elementos del archivo ajenos al normalizador y a los ajustes de cálculo se preservaron antes de actualizar únicamente los resultados almacenados. No se modificaron los valores de entrada, las imágenes, los gráficos, las validaciones ni las fórmulas del resto del libro.
7. Proyecto VBA conservado byte por byte. Su hash es `1edf2efc0dab927a2a09b0864835125a4250d614044d45da3649fd738ab60744`. No se ejecutaron las macros ni se simuló la interfaz de Microsoft Excel.

## Abrir y usar

Cerrar la copia anterior y abrir esta versión nueva en **Excel de escritorio**, especialmente para el cambio automático de fotos mediante VBA. SharePoint puede almacenar y descargar el XLSM; Excel para la Web no ejecuta macros. Los controles de datos de origen se mantienen: no se sustituyeron faltantes por cifras inventadas ni se ocultaron avisos.

No se probó el inicio de sesión, la subida ni la descarga en el sitio SharePoint. El paquete V3 incorpora esta mensual optimizada y conserva las otras tres planillas de la entrega V2.

SHA-256 de la entrega: `59ea7640dae8eba3bb7d1c9291b8f99cbca25218124651f854f8e66b379c1abd`.
