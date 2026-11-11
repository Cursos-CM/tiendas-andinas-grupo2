---
agent: 'agent'
description: 'Crear un rol de seguridad por filas (RLS), con plan y aprobación'
argument-hint: 'Nombre del rol y filtro, por ejemplo: Región Caribe, tiendas de la región Caribe'
---
Rol pedido: ${input:rol}

CONTEXTO: Modelo TiendasAndinas abierto en Power BI Desktop. Las tiendas están en la tabla tbl_Tienda.
OBJETIVO: Crear un rol de seguridad por filas que deje ver solo las filas pedidas.
RESTRICCIONES:
- Usa solo la herramienta security_role_operations del servidor MCP. No edites archivos .tmdl.
- Un rol tiene dos partes y hacen falta las dos: el rol (operación Create, con ModelPermission Read) y el permiso de tabla con el filtro (operación CreatePermissions, con RoleName, TableName y FilterExpression). Si el rol ya existe, no lo vuelvas a crear: crea o actualiza solo el permiso de tabla (CreatePermissions o UpdatePermissions).
- Un único filtro DAX sobre una tabla de dimensión. No cambies medidas, relaciones ni otros roles.
- No ejecutes nada hasta que escriba APROBADO.
FORMATO:
1. Primero, el plan en una tabla: nombre del rol, permiso, tabla filtrada, expresión DAX del filtro y qué tablas de hechos quedan filtradas por las relaciones.
2. Cuando escriba APROBADO, haz las dos operaciones y después comprueba con ListPermissions del rol que el permiso de tabla existe y tiene el filtro. Muéstrame esa comprobación. Si el permiso no aparece, dilo claramente: no digas que el rol quedó listo.
3. Termina diciéndome cómo probarlo en Power BI Desktop con Modelado → Ver como.
CRITERIO: ListPermissions muestra el filtro y, con Ver como, el informe muestra solo las filas del filtro.
