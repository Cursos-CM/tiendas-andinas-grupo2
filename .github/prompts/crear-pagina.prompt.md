---
agent: 'agent'
description: 'Crear mi página del informe a partir de mi encargo, con plan y aprobación'
argument-hint: 'Su nombre y su número de encargo, por ejemplo: Ana, encargo 4'
---
Datos: ${input:datos}

CONTEXTO: Proyecto PBIP TiendasAndinas. Los encargos están en ENCARGOS.md. Las páginas del informe están en TiendasAndinas.Report/definition/pages.
OBJETIVO: Crear una página nueva del informe llamada «Página de <nombre>» con los dos visuales de mi encargo: el gráfico principal y la tarjeta.
RESTRICCIONES:
- Usa como plantilla los page.json y visual.json de la página Resumen. Para un tipo de gráfico que no esté en Resumen, adapta la plantilla más parecida.
- Crea solo archivos nuevos dentro de una carpeta nueva para mi página. No modifiques pages.json, el modelo semántico ni otras páginas.
- El título del gráfico es el nombre del encargo seguido de mi nombre entre paréntesis.
FORMATO:
1. Primero, el plan: una tabla con cada archivo que vas a crear y qué contiene (tipo de visual, campos, título, posición). NO crees nada todavía.
2. Cuando escriba APROBADO, crea los archivos y termina con el nombre de la carpeta de mi página.
CRITERIO: La página debe abrir en Power BI Desktop sin errores y mostrar los valores esperados de ENCARGOS.md.
