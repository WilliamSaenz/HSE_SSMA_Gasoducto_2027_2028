# Semanal PC — V5 corregida

Usar [Planilla_Semanal_Planta_C_HSE_V5_CORREGIDA.xlsx](Planilla_Semanal_Planta_C_HSE_V5_CORREGIDA.xlsx). Reemplaza a la V4, que tenía errores de estructura al abrir en Excel.

Se corrigió el orden de las propiedades de cuatro fuentes y se quitaron de la copia oculta de respaldo los vínculos duplicados a objetos que pertenecen a la hoja original. Se retiró también su identificador de revisión duplicado. La tabla, comentarios y objetos originales siguen en su hoja original.

Todas las celdas, fórmulas, validaciones, datos, fotografías y el formato de las hojas de carga se conservaron. Se compararon los contenidos de todas las hojas antes y después; el cambio se limita al archivo de estilos y a la estructura del respaldo oculto.

Validación con el SDK oficial Microsoft DocumentFormat.OpenXml 3.3.0:

- Esquema Microsoft 365: **0 errores**.
- Esquema Office 2021: **0 errores**.
- Integridad del paquete ZIP: correcta.
- Fotografías y objetos enriquecidos: idénticos a V4.

Las instrucciones de carga y las funciones de conciliación son las de [la guía del semanal](LEEME_PC_V4.md). La corrección es de estructura; no cambia los valores ni completa los datos operativos pendientes.

SHA256 del Excel V5: `3105080815bbc5237e1425e1c6d71fe1fd04af487c9430e230850e122c90ad15`.
