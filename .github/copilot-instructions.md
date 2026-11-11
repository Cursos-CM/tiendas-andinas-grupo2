# Instrucciones del equipo Tiendas Andinas para GitHub Copilot

## Contexto
- Repositorio compartido del equipo: proyecto PBIP **TiendasAndinas** (retail ficticio, Colombia, datos 2024–2025).
- `TiendasAndinas.SemanticModel` es el modelo semántico (TMDL). `TiendasAndinas.Report` es el informe (PBIR): cada página es una carpeta en `TiendasAndinas.Report/definition/pages`, con su `page.json` y una carpeta `visuals` con un `visual.json` por visual.
- Cada integrante del equipo construye **una página propia** del informe y la entrega con un pull request.

## Idioma y estilo
- Responde siempre en español, de forma concisa.
- Presenta planes, resultados y listas de archivos como tablas en Markdown.

## Reglas del equipo (obligatorias)
1. **El modelo semántico se cambia solo con el servidor MCP**, nunca editando los archivos de `TiendasAndinas.SemanticModel`. Los cambios al modelo no se suben en las ramas de página: los integra el dueño del modelo en un pull request propio.
2. **En el informe, cada persona trabaja solo en la carpeta de su página.** No modifiques `pages.json`, `report.json`, `version.json`, `definition.pbir` ni las páginas de otras personas.
3. Antes de cambiar el modelo o crear o cambiar archivos, presenta un **plan** (archivos que vas a crear o cambiar y qué contiene cada uno) y **espera a que escriba APROBADO**.
4. Para crear una página o un visual, usa como plantilla los `page.json` y `visual.json` de la página **Resumen**. Los nombres de carpeta nuevos deben ser de 20 caracteres hexadecimales en minúscula y no deben existir ya en el proyecto.
5. Usa solo tablas, columnas y medidas que existan en el modelo, con sus nombres exactos.
6. Los títulos de los visuales van en español y terminan con el nombre de la persona entre paréntesis, por ejemplo «Ventas por canal (Ana)».
7. No incluyas en respuestas ni archivos contraseñas, tokens ni datos personales.

## Consultas al modelo
- Para consultar datos, conéctate al archivo TiendasAndinas abierto en Power BI Desktop y usa solo operaciones de lectura (List, Get y consultas DAX).
- Muéstrame la consulta DAX antes de ejecutarla.
- Si no encuentras ninguna instancia de Power BI Desktop, lee el número del archivo msmdsrv.port.txt que está en %LOCALAPPDATA%\Microsoft\Power BI Desktop\AnalysisServicesWorkspaces (subcarpeta Data) y conéctate a localhost con ese puerto.

## Después de crear o cambiar una página
- Recuérdame que Power BI Desktop no ve los cambios en vivo: hay que cerrarlo **sin guardar** y volver a abrir `TiendasAndinas.pbip`.
- Dime el nombre de la carpeta de mi página: es la que voy a subir a GitHub.
