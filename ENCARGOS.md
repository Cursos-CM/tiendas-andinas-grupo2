# Encargos de la gerencia de Tiendas Andinas

Cada integrante construye una página con **dos visuales**: el gráfico principal y una tarjeta. Su número de encargo es su número en la lista de asistencia; del 13 en adelante, vuelva a empezar (13 → 1, 14 → 2…).

Los valores esperados son del total de los datos (2024 y 2025), sin filtros.

| # | Encargo | Gráfico principal | Tarjeta | Valores esperados para validar |
|---|---|---|---|---|
| 1 | Ventas por canal | Columnas: `Total Ventas` por `FACT_Ventas[Canal]` | `Ticket Promedio` | Tienda 8.380.537.525 · Online 3.028.987.545 · Ticket 553.350 |
| 2 | Ventas por región | Barras: `Total Ventas` por `tbl_Tienda[Region]` | `# Clientes` | Online 3.028.987.545 · Centro 2.174.714.870 · Clientes 2.375 |
| 3 | Ventas por tipo de tienda | Columnas: `Total Ventas` por `tbl_Tienda[Tipo]` | `# Órdenes` | Flagship 4.359.162.200 · Online 3.028.987.545 · Órdenes 20.619 |
| 4 | Devoluciones por motivo | Barras: `Unidades Devueltas` por `fact_devoluciones[Motivo]` | `Tasa Devolucion` | Cambio de opinión 626 · Producto defectuoso 556 · Tasa 5,7 % |
| 5 | Margen por categoría | Columnas: `Margen %` por `Categoria[Categoria]` | `Margen %` | Deportes 35,7 % · Tecnología 33,0 % · Margen total 33,6 % |
| 6 | Cumplimiento por categoría | Barras: `Cumplimiento` por `Categoria[Categoria]` | `Diferencia vs Presupuesto` | Moda 98,4 % · Tecnología 97,4 % · Diferencia −259.136.930 |
| 7 | Clientes por segmento | Columnas: `# Clientes` por `Cliente[Segmento]` | `Ticket Promedio` | Ocasional 1.144 · Corporativo 175 · Ticket 553.350 |
| 8 | Ventas por día de la semana | Columnas: `Total Ventas` por `Calendario[DiaSemana]` | `Unidades Vendidas` | sábado 1.811.865.555 · viernes 1.395.537.450 · Unidades 51.780 |
| 9 | Ventas por trimestre | Columnas: `Total Ventas` por `Calendario[Trimestre]` | `Ventas Online` | T4 3.653.762.355 · T1 2.241.575.370 · Online 3.028.987.545 |
| 10 | Ventas por departamento del cliente | Barras: `Total Ventas` por `Cliente[Departamento]` | `# Clientes` | Cundinamarca 2.105.824.195 · Meta 1.002.506.720 · Clientes 2.375 |
| 11 | Tendencia mensual | Líneas: `Total Ventas` por `Calendario[AnioMes]` | `Total Ventas` | 2025-12 811.096.045 · 2024-02 310.180.520 · Total 11.409.525.070 |
| 12 | Unidades por categoría | Barras: `Unidades Vendidas` por `Categoria[Categoria]` | `Tasa Devolucion` | Moda 28.327 · Deportes 5.099 · Tasa 5,7 % |
