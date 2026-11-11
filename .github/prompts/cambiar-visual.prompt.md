---
agent: 'agent'
description: 'Cambiar un visual de mi página: tipo, título, campos o tamaño'
argument-hint: 'Su nombre y el cambio, por ejemplo: Ana, cambia el gráfico a barras'
---
Cambio pedido: ${input:cambio}

CONTEXTO: Proyecto PBIP TiendasAndinas. Mi página es la carpeta de TiendasAndinas.Report/definition/pages cuyo page.json tiene displayName «Página de <mi nombre>».
OBJETIVO: Aplicar el cambio pedido en el visual.json que corresponda.
RESTRICCIONES: Cambia solo archivos de la carpeta de mi página. No modifiques pages.json, el modelo semántico ni otras páginas. Si el cambio requiere una medida o columna que no existe, dilo y no lo hagas.
FORMATO: Antes de cambiar, muéstrame en una tabla qué propiedad cambia, con el valor actual y el nuevo, y espera a que escriba APROBADO.
CRITERIO: Después del cambio, el visual debe seguir abriendo en Power BI Desktop sin errores.
