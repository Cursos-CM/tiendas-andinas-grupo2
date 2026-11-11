# Tiendas Andinas · Informe del equipo

Repositorio de práctica del Día 4 del curso «Modelado semántico de Power BI asistido por IA con GitHub Copilot y MCP».

Todo el equipo trabaja sobre el **mismo proyecto PBIP**. Cada persona agrega **una página** al informe y la entrega con un **pull request**. Al final, la rama `main` tiene el informe completo del equipo.

## Qué hay en el repositorio

| Carpeta o archivo | Para qué sirve |
|---|---|
| `TiendasAndinas.pbip` | Abre el proyecto en Power BI Desktop |
| `TiendasAndinas.SemanticModel` | El modelo semántico (TMDL). Lo integra solo el dueño del modelo, en su propio pull request |
| `TiendasAndinas.Report/definition/pages` | Las páginas del informe (PBIR): una carpeta por página |
| `ENCARGOS.md` | Los 12 encargos de la gerencia, con los valores esperados |
| `.github/copilot-instructions.md` | Las reglas del equipo para Copilot |
| `.github/prompts` | Los prompts del equipo: `/consultar-encargo`, `/documentar-medidas`, `/crear-rol`, `/crear-pagina` y `/cambiar-visual` |
| `.github/pull_request_template.md` | La plantilla que aparece al abrir un pull request |

## Reglas del equipo

1. Nadie sube cambios directo a `main`: todo entra por pull request.
2. Cada persona trabaja en su rama: `pagina-su-nombre` (minúsculas, sin tildes ni espacios).
3. Cada pull request de página agrega **solo la carpeta de esa página**. No se suben `pages.json`, `report.json` ni archivos del modelo: los cambios al modelo los sube el dueño del modelo.
4. Antes de aprobar, otra persona revisa el pull request.

## Flujo de trabajo

```text
main ──●──────────────────────────────●── (informe del equipo)
        \                            /
         ●── pagina-ana ── PR ── revisión ── merge
```

1. En su equipo, con Copilot: documentar el modelo, crear el rol de seguridad, construir la página y validarla en Power BI Desktop.
2. Crear la rama `pagina-su-nombre` desde `main`.
3. Subir la carpeta de la página a su rama (**Add file → Upload files**).
4. Abrir el pull request y pedir revisión.
5. Cuando esté aprobado, el instructor lo integra (merge) en `main`.

Los datos se leen de `C:\CursoPBI\Datos`, la carpeta que instaló el paquete del curso.
