---
agent: 'agent'
description: 'Documentar en un solo lote todas las medidas del modelo, con plan y aprobación'
---
CONTEXTO: Modelo TiendasAndinas abierto en Power BI Desktop.
OBJETIVO: Escribir una descripción de negocio para cada medida del modelo, en una sola operación masiva.
RESTRICCIONES:
- Usa solo las herramientas del servidor MCP. No edites archivos .tmdl.
- Cambia únicamente la descripción de las medidas: no cambies nombres, expresiones, formatos ni carpetas.
- No ejecutes nada hasta que escriba APROBADO.
FORMATO:
1. Primero, el plan: una tabla con medida, carpeta y descripción propuesta (máximo 20 palabras, en lenguaje de negocio, sin fórmulas).
2. Cuando escriba APROBADO, aplica todas las descripciones en un solo lote y termina con el número de medidas actualizadas.
CRITERIO: Deben quedar descritas todas las medidas del modelo (son 18).
