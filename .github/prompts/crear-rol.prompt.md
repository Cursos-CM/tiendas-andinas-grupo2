---
agent: 'agent'
description: 'Crear un rol de seguridad por filas (RLS), con plan y aprobación'
argument-hint: 'Nombre del rol y filtro, por ejemplo: Región Caribe, tiendas de la región Caribe'
---
Rol pedido: ${input:rol}

CONTEXTO: Modelo TiendasAndinas abierto en Power BI Desktop. Las tiendas están en la tabla tbl_Tienda.
OBJETIVO: Crear un rol de seguridad por filas que deje ver solo las filas pedidas.
RESTRICCIONES:
- Usa solo las herramientas del servidor MCP. No edites archivos .tmdl.
- Permiso de lectura y un único filtro DAX sobre una tabla de dimensión. No cambies medidas, relaciones ni otros roles.
- No ejecutes nada hasta que escriba APROBADO.
FORMATO:
1. Primero, el plan en una tabla: nombre del rol, permiso, tabla filtrada, expresión DAX del filtro y qué tablas de hechos quedan filtradas por las relaciones.
2. Cuando escriba APROBADO, crea el rol y dime cómo probarlo en Power BI Desktop y qué valor de Total Ventas debería verse con el rol.
CRITERIO: El rol aparece en Modelado → Administrar roles y, con Ver como, el informe muestra solo las filas del filtro.
