---
agent: 'agent'
description: 'Consultar en el modelo los datos de un encargo, sin cambiar nada'
argument-hint: 'Número de encargo, por ejemplo: 4'
---
Encargo: ${input:encargo}

CONTEXTO: Proyecto TiendasAndinas abierto en Power BI Desktop. Los encargos están en el archivo ENCARGOS.md de este repositorio.
OBJETIVO: Comprobar con datos el encargo indicado antes de construir la página.
RESTRICCIONES: No cambies nada: ni el modelo ni ningún archivo. Usa solo operaciones de lectura.
FORMATO:
1. Lee la fila del encargo en ENCARGOS.md.
2. Muéstrame una consulta DAX con SUMMARIZECOLUMNS que calcule la medida del gráfico por su columna, y otra con la medida de la tarjeta. Ejecútalas.
3. Responde con una tabla de resultados ordenada de mayor a menor y una línea final que diga si coinciden con los valores esperados de ENCARGOS.md.
CRITERIO: Máximo 25 filas. Si una tabla, columna o medida no existe, dilo y no inventes nombres.
