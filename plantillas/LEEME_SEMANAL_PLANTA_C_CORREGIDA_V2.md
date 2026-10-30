# Semanal Planta Compresora corregida V2

Base: último adjunto BORRADOR_Semanal_Planta_C.xlsx. Se conserva la agrupación OPS/SMP y las filas eliminadas por el usuario no se restituyen.

- Reparadas 60 fórmulas con referencias eliminadas. Los controles de carga ahora consideran 26 campos obligatorios por semana, en lugar de 30.
- Los kilómetros consolidados se contrastan con OPS + SMP; las inconsistencias se señalan sin alterar los valores ingresados.
- En BD_SEMANAL, 24 registros del detalle eliminado YPF/PAE quedan vacíos, para evitar duplicar SMP. Doce registros vigentes se identifican como SMP. No se modificó el detalle de ICM por empresa.
- Las tarjetas se limitan al mes seleccionado, aunque las semanas crucen sus límites. Se corrigieron el mes de control y el aviso de fechas fuera del mes. Se conservan las metas SMP 6 y OPS 1 y la carga manual recibida de 113 tarjetas; sin listado nominal no se inventa un porcentaje de cumplimiento.
- Fechas completas con formato día/mes/año. Se conservan formatos de mes y horarios donde corresponden.
- La hoja 03_TARJETAS_OBSERVACION queda sin protección. Las demás hojas y la estructura están protegidas con la clave acordada, manteniendo habilitadas las entradas existentes.
- Se actualizaron los resultados calculados conservando las fórmulas y los objetos originales. Cálculo automático, sin forzar el recálculo completo en cada apertura.

Validación: 87 hojas y 245.823 fórmulas; recálculo independiente sin errores de celda. Pruebas de kilómetros coherentes/incoherentes, metas SMP/OPS, exclusión de tarjetas fuera del mes y carga en la última fila 1510 satisfactorias. Los datos literales del usuario se conservaron; solo cambió el rótulo del control de 30 a 26. Imágenes y dibujos conservados. No se guardó el archivo final mediante conversión de LibreOffice.

Siguen pendientes los datos que no estaban completados: kilómetros, períodos semanales que requieren revisión, identificación/clasificación de observaciones y responsables de acciones. Se conservan sus avisos; cero errores de fórmula no significa que la información esté completa.

Preparada para cargar en SharePoint: sin vínculos a otros libros ni conexiones externas de datos. Se conservan los hipervínculos normales. No se realizó una carga ni descarga real en SharePoint ni una prueba de apertura con Microsoft Excel de escritorio; esas comprobaciones requieren el servicio y la aplicación correspondientes.
