# Biblioteca de skills

Skills independientes para trabajar con interfaces. Cada carpeta contiene su propio `SKILL.md` y los recursos que necesita.

| Skill | Propósito | Dependencias |
| --- | --- | --- |
| [preview-components](preview-components/SKILL.md) | Comparar tres propuestas visuales y aplicar la elección del usuario. | Skill Impeccable instalada por separado. |
| [interface-design](interface-design/SKILL.md) | Crear, auditar o corregir interfaces interpretando intención y contexto. | Ninguna skill externa. |

`interface-design` aporta criterios de diseño. `preview-components` aporta un flujo de exploración; guardar ambas en el repositorio no obliga a ejecutar siempre las dos.

## Instalación en Codex

Copia la carpeta completa de la skill deseada en `$CODEX_HOME/skills`; si no se ha definido `CODEX_HOME`, usa `~/.codex/skills`. Conserva sus subcarpetas. Comprueba si ya existe antes de copiar y revisa los cambios antes de sustituir una versión local.

Abre una nueva sesión si la skill todavía no aparece en el catálogo. Puedes invocarla como `$interface-design` o `$preview-components`; ambas permiten selección automática cuando corresponde al encargo.

## Añadir nuevas skills

Crea una carpeta independiente con nombre en minúsculas y guiones, un `SKILL.md` con `name` y `description`, y únicamente los recursos necesarios. Añade su propósito y dependencias a este catálogo. No incluyas credenciales, archivos privados de proyectos ni dependencias voluminosas.
