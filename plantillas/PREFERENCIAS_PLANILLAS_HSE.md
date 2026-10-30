# Preferencias vigentes de William para las planillas HSE

Confirmadas el 30/10/2026. Aplicar en futuras revisiones de las otras planillas cuando exista el campo correspondiente; las instrucciones nuevas del usuario prevalecen.

- Usar estos rótulos para las observaciones mensuales:
  - `Observaciones de comportamiento: abiertas (Total: OPS+SMP) / mes`
  - `Observaciones de comportamiento seguro: cerradas y positivas` y en la segunda línea `(Total: OPS+SMP) /mes`.
- Dejar la solapa `Tarjetas_Observacion` completamente **sin protección de hoja**, para permitir su futura automatización con datos de otras planillas. Mantener protegidas las demás hojas/fórmulas y la estructura salvo instrucción distinta; conservar editables las celdas de carga.
- Si la versión recibida no contiene esa solapa, informar la ausencia. Puede prepararse una hoja vacía para la integración futura; no afirmar que se recuperaron datos ni crear vínculos o registros sin una fuente definida.
- Usar siempre el último archivo del usuario como base, preservando sus ediciones. No restituir valores borrados desde versiones anteriores sin respaldo.
- La clave de protección fue suministrada por el usuario en la conversación. No guardarla en texto en este documento, en scripts publicados ni en descripciones.

Aplicación actual: `Plantilla_KPIs_PC_V7_TARJETAS_LIBRE.xlsx`. La versión mensual previa no contenía Tarjetas_Observacion; en V7 se agregó vacía, sin protección, con encabezados para futura integración. No hay enlaces automáticos todavía.

Aplicación Ducto: `Plantilla_KPIs_Ducto_V6_CORREGIDA_PROTEGIDA.xlsm`. Mantener el alcance **UT+SMP** del Ducto (UT: SICIM + VC), sin copiar el nombre OPS propio de la Planta. Tarjetas_Observacion ya existía y se conservó sin protección, con sus fórmulas y registros.
